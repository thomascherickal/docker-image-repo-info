## `maven:3-amazoncorretto-8`

```console
$ docker pull maven@sha256:0a1834b9a003164a68bb915b1d954b3dc75987b56eb5cd582e7ec435ec1f67c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8` - linux; amd64

```console
$ docker pull maven@sha256:386ae57ad33b110c27183c583b42f23a191cefe79d56c4ceb42a3cb4badae161
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.2 MB (150226401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924e11c8ab41f6687013749199ac372860b977aaf2703027ae3c49cab7eb434c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 22 Sep 2022 19:19:21 GMT
ADD file:99847692b0f2dee43b50f306ad92fbc13ccb0541af21c6d3040f72d3184aabac in / 
# Thu, 22 Sep 2022 19:19:21 GMT
CMD ["/bin/bash"]
# Tue, 18 Oct 2022 23:36:48 GMT
ARG version=1.8.0_352.b08-1
# Tue, 18 Oct 2022 23:37:10 GMT
# ARGS: version=1.8.0_352.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 18 Oct 2022 23:37:10 GMT
ENV LANG=C.UTF-8
# Tue, 18 Oct 2022 23:37:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 19 Oct 2022 00:11:49 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 19 Oct 2022 00:11:49 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 19 Oct 2022 00:11:49 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2022 00:11:49 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 19 Oct 2022 00:11:49 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 19 Oct 2022 00:11:55 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2022 00:11:56 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2022 00:11:56 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2022 00:11:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 19 Oct 2022 00:11:56 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2022 00:11:56 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 19 Oct 2022 00:11:56 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2022 00:11:56 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e80285ff599e329e689e4689be05885456823b7f6233486aa419541ae8e98c62`  
		Last Modified: Wed, 21 Sep 2022 22:07:12 GMT  
		Size: 62.3 MB (62303269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f29b7e60081ce18a48e94227aad7abe07354efb88b76714cede956e903ce336`  
		Last Modified: Tue, 18 Oct 2022 23:43:46 GMT  
		Size: 75.6 MB (75558393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2012f0a2edbd8444df60854511044e44b9ece01b0c2b8353c6f86703f699dc20`  
		Last Modified: Wed, 19 Oct 2022 00:14:45 GMT  
		Size: 3.6 MB (3624008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e076c75faea06d218a64648e1c323eeaf77394f78e539e59f978439e25439343`  
		Last Modified: Wed, 19 Oct 2022 00:14:45 GMT  
		Size: 8.7 MB (8739515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff054b180af1699e2e03e819f49e4fa3b66fa7357518023676778c0e2c25125`  
		Last Modified: Wed, 19 Oct 2022 00:14:44 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ada59152208314a268355cc7d20fe85ae279c18211da8d7f67c0c637e33461d`  
		Last Modified: Wed, 19 Oct 2022 00:14:44 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:ea0afb61d69ad029c554d8c85fb631b30b0a60b78d2dd14c355ed8c8da5e70be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.9 MB (135856790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e14131c1f7772375d7c3f15a46b8f8a15d97884f46a5ac0f6316f633c8558b5`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 22 Sep 2022 19:39:26 GMT
ADD file:cd0852de8cdfb2b7efdaa53ad4827a33302d895b10306b540e7df9d8c7f00637 in / 
# Thu, 22 Sep 2022 19:39:27 GMT
CMD ["/bin/bash"]
# Wed, 19 Oct 2022 00:34:04 GMT
ARG version=1.8.0_352.b08-1
# Wed, 19 Oct 2022 00:34:17 GMT
# ARGS: version=1.8.0_352.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 19 Oct 2022 00:34:17 GMT
ENV LANG=C.UTF-8
# Wed, 19 Oct 2022 00:34:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 19 Oct 2022 01:25:28 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 19 Oct 2022 01:25:29 GMT
ARG MAVEN_VERSION=3.8.6
# Wed, 19 Oct 2022 01:25:30 GMT
ARG USER_HOME_DIR=/root
# Wed, 19 Oct 2022 01:25:31 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Wed, 19 Oct 2022 01:25:32 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Wed, 19 Oct 2022 01:25:35 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 19 Oct 2022 01:25:36 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 19 Oct 2022 01:25:37 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 19 Oct 2022 01:25:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 19 Oct 2022 01:25:40 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 19 Oct 2022 01:25:41 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 19 Oct 2022 01:25:41 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 19 Oct 2022 01:25:42 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:f5371f42f94d8ba2c9559448b8e36de82d246f179760ec911f594632d3545611`  
		Last Modified: Wed, 21 Sep 2022 22:07:11 GMT  
		Size: 63.9 MB (63912418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff798ab4b40b7a00ffb17ba557ffb7327b504857ea8b7cb1773e85ddc8141346`  
		Last Modified: Wed, 19 Oct 2022 00:36:31 GMT  
		Size: 59.6 MB (59581110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42326b9ca1185c500787392dfba926f50b3be6852e66d6617081ed2fa3f27f6`  
		Last Modified: Wed, 19 Oct 2022 01:29:20 GMT  
		Size: 3.6 MB (3622581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8befcf6db3b2abb932b39facffbee3a8de61c799e97e4962c71ff0afaa35b3f3`  
		Last Modified: Wed, 19 Oct 2022 01:29:20 GMT  
		Size: 8.7 MB (8739469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63d265af3214a2a0980f41b23f092fba0968202a97bd1aaab3f0adc39b82a52`  
		Last Modified: Wed, 19 Oct 2022 01:29:19 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062aa89d0c0d87f17b955f142ea90cdae8b55f3690b5312c5b0a7cbb50fe8411`  
		Last Modified: Wed, 19 Oct 2022 01:29:19 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
