## `maven:3-amazoncorretto-15`

```console
$ docker pull maven@sha256:ee5f660324710f6f5115f097788755d136a3f0576fc86cd6966c1456bb9a719a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-15` - linux; amd64

```console
$ docker pull maven@sha256:336e29025918ed4ce397a48fd8706461d5b90394eb28874581a819cee1ea9036
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230759049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ceeab9b8fe03317e81f720d20a66b3cd2a121d98c6996975f7eff7921a732de`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 24 Feb 2021 19:19:48 GMT
ADD file:40bc6ac9b95149d9077e8e692feea2208fcd1c5883673953b295e6acd014ea38 in / 
# Wed, 24 Feb 2021 19:19:48 GMT
CMD ["/bin/bash"]
# Wed, 24 Feb 2021 19:37:52 GMT
ARG version=15.0.2.7-1
# Wed, 24 Feb 2021 19:38:11 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 24 Feb 2021 19:38:11 GMT
ENV LANG=C.UTF-8
# Wed, 24 Feb 2021 19:38:12 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
# Wed, 24 Feb 2021 19:57:24 GMT
ARG MAVEN_VERSION=3.6.3
# Wed, 24 Feb 2021 19:57:25 GMT
ARG USER_HOME_DIR=/root
# Wed, 24 Feb 2021 19:57:25 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Wed, 24 Feb 2021 19:57:25 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Wed, 24 Feb 2021 19:57:31 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 24 Feb 2021 19:57:33 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 24 Feb 2021 19:57:33 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 24 Feb 2021 19:57:33 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 24 Feb 2021 19:57:34 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 24 Feb 2021 19:57:34 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 24 Feb 2021 19:57:34 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 24 Feb 2021 19:57:34 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:9da98c321efd693e1dc19cc24c7c2cfa365c649f178da8ebdfdc5243d0b2f91a`  
		Last Modified: Wed, 24 Feb 2021 10:37:31 GMT  
		Size: 61.9 MB (61935160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a8cdca3ea041af86978577d8c0516ea483e3803a7ac7baed759a049f0d3ad9`  
		Last Modified: Wed, 24 Feb 2021 19:40:06 GMT  
		Size: 155.7 MB (155668468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1db2eca3cf32cc88cdd40b7bf760adce65cfd463856d727902ab27df7604d69`  
		Last Modified: Wed, 24 Feb 2021 20:00:14 GMT  
		Size: 3.6 MB (3572980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa04f9951257b5429f9e5ca91112540e24f3b0da94df36454452ec82e5d0efc9`  
		Last Modified: Wed, 24 Feb 2021 20:00:12 GMT  
		Size: 9.6 MB (9581228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef45152e48282a4639e6cb075b2370e14c067c07db123656aba82a1911df805`  
		Last Modified: Wed, 24 Feb 2021 20:00:13 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda33e4029da8cf3dc1ca24471b83c4532b29268cfd34610d3901d7f64f86187`  
		Last Modified: Wed, 24 Feb 2021 20:00:11 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-15` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:6cc5b633c2fe93282b53a6c6b31055914a5f15904424b16be4ba5e25f06415b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232422722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e16e6372d7b6fb10867728ce0de824711cceeb5d39768d3c63ddce21290a3713`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 27 Jan 2021 23:09:56 GMT
ADD file:7f69686262e0e0e5415d42ac0371f7d0df0330bc4f0556e5d4b73dd78ceb1197 in / 
# Wed, 27 Jan 2021 23:10:02 GMT
CMD ["/bin/bash"]
# Wed, 27 Jan 2021 23:49:30 GMT
ARG version=15.0.2.7-1
# Wed, 27 Jan 2021 23:50:00 GMT
# ARGS: version=15.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 27 Jan 2021 23:50:02 GMT
ENV LANG=C.UTF-8
# Wed, 27 Jan 2021 23:50:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
# Thu, 28 Jan 2021 00:25:36 GMT
ARG MAVEN_VERSION=3.6.3
# Thu, 28 Jan 2021 00:25:36 GMT
ARG USER_HOME_DIR=/root
# Thu, 28 Jan 2021 00:25:37 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Thu, 28 Jan 2021 00:25:38 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Thu, 28 Jan 2021 00:25:49 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Thu, 28 Jan 2021 00:25:54 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 28 Jan 2021 00:25:56 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 28 Jan 2021 00:25:57 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 28 Jan 2021 00:25:57 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 28 Jan 2021 00:25:58 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 28 Jan 2021 00:25:59 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 28 Jan 2021 00:25:59 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:c6741bcf27a42820ff66e35cc842cec9a845e9e9dba4ff7bd465fc6161442a86`  
		Last Modified: Wed, 27 Jan 2021 23:11:10 GMT  
		Size: 63.7 MB (63704713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68666620335f38cf95ebec188e1b987827b8bac236561b2eda344ccef1ecd47`  
		Last Modified: Wed, 27 Jan 2021 23:52:01 GMT  
		Size: 155.5 MB (155544910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb6debee19b27bce30c378ac19163128748b26c37c7c5926e66aeb3e1ef51c9`  
		Last Modified: Thu, 28 Jan 2021 00:28:36 GMT  
		Size: 3.6 MB (3590689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a9ba3fc52e6676554dea16d7b5eea9671c147c4579b000d89e72b58999f9c0`  
		Last Modified: Thu, 28 Jan 2021 00:28:36 GMT  
		Size: 9.6 MB (9581194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a607a3c0857fe3baeb73fba5cad944bf050f2fe401ab28f6f3f965a76f5de820`  
		Last Modified: Thu, 28 Jan 2021 00:28:35 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ee09049d1c0456d68a132e4989c2a064626ffe3453d04720a18f3d499af6b8`  
		Last Modified: Thu, 28 Jan 2021 00:28:35 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
