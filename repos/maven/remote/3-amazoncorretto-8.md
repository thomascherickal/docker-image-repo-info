## `maven:3-amazoncorretto-8`

```console
$ docker pull maven@sha256:9ab5af332ed75defe887ccc326e5784a7772ed6c7dd11f3dbb08cbfd3e8d4c6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8` - linux; amd64

```console
$ docker pull maven@sha256:2641801ebc5cb00bed675a40ebb2265787fdd8a969638c28fa7d9dee1503c715
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.3 MB (150250230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d37a92bb96133edb7c5f8c8f5c77d3e338fb8e9ec34ae1857f443077e3d752f9`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 16 Dec 2022 01:19:49 GMT
ADD file:a69ca7a5499bcd9d6e4317fdbd7256e93be44364bb746f5da10b4268c090bda0 in / 
# Fri, 16 Dec 2022 01:19:50 GMT
CMD ["/bin/bash"]
# Fri, 16 Dec 2022 02:12:29 GMT
ARG version=1.8.0_352.b08-1
# Fri, 16 Dec 2022 02:13:02 GMT
# ARGS: version=1.8.0_352.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Dec 2022 02:13:03 GMT
ENV LANG=C.UTF-8
# Fri, 16 Dec 2022 02:13:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 16 Dec 2022 03:12:47 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 16 Dec 2022 03:12:47 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 16 Dec 2022 03:12:47 GMT
ARG USER_HOME_DIR=/root
# Fri, 16 Dec 2022 03:12:47 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 16 Dec 2022 03:12:47 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 16 Dec 2022 03:12:48 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 16 Dec 2022 03:12:48 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 16 Dec 2022 03:12:49 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 16 Dec 2022 03:12:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 16 Dec 2022 03:12:49 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 16 Dec 2022 03:12:49 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 16 Dec 2022 03:12:49 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 16 Dec 2022 03:12:49 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5b4a36b5b78f93a5f470cf722b313bb32cddb0f8e0fa0db348059b5c0881b04f`  
		Last Modified: Thu, 15 Dec 2022 23:08:20 GMT  
		Size: 62.3 MB (62328625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898f795353afe49c938db3ca88457ed5e0aaa4e3c5cad075d569dee85e2f54ab`  
		Last Modified: Fri, 16 Dec 2022 02:20:57 GMT  
		Size: 75.6 MB (75560173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd84c6f1e133ebfeffd341a5ce76976970783ad1821ed9536cc2a6a4389a99a`  
		Last Modified: Fri, 16 Dec 2022 03:15:33 GMT  
		Size: 3.6 MB (3620722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f23131bd79125201e4428c93ba48163ca294e348c57b5df88ebcf33ed4291cd`  
		Last Modified: Fri, 16 Dec 2022 03:15:33 GMT  
		Size: 8.7 MB (8739503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb119f803d638cab74d83728eda83c8846ab7cc25dbf8658aae6efa73febc0a`  
		Last Modified: Fri, 16 Dec 2022 03:15:32 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb045e564cec6c7d84c22e0d82a744cc301ae60bf5dd7c61ce414eedf96730d`  
		Last Modified: Fri, 16 Dec 2022 03:15:32 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:8e2516f07d5ae6c53c0d3ec575ebfbcf4aed9ebeea4d24a1aa4b5a3ca994f96f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.9 MB (135939674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b884ba82d0d910c759097b9344c7da6fdbef2402ebefbdbd9e28f9689108a7aa`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 16 Dec 2022 00:41:05 GMT
ADD file:26a6bf75c84c408d289e5569f13b1c65206966f875cdfc53ded0670cb85e35bf in / 
# Fri, 16 Dec 2022 00:41:07 GMT
CMD ["/bin/bash"]
# Fri, 16 Dec 2022 00:58:43 GMT
ARG version=1.8.0_352.b08-1
# Fri, 16 Dec 2022 00:58:59 GMT
# ARGS: version=1.8.0_352.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Dec 2022 00:59:00 GMT
ENV LANG=C.UTF-8
# Fri, 16 Dec 2022 00:59:00 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 16 Dec 2022 01:23:06 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 16 Dec 2022 01:23:06 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 16 Dec 2022 01:23:07 GMT
ARG USER_HOME_DIR=/root
# Fri, 16 Dec 2022 01:23:07 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 16 Dec 2022 01:23:07 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 16 Dec 2022 01:23:14 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 16 Dec 2022 01:23:14 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 16 Dec 2022 01:23:14 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 16 Dec 2022 01:23:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 16 Dec 2022 01:23:14 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 16 Dec 2022 01:23:14 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 16 Dec 2022 01:23:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 16 Dec 2022 01:23:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:6cbfee25f0741b3d3f4d2474d904a200cd8404a01aa17813bf3fc3d4ebb551a4`  
		Last Modified: Thu, 15 Dec 2022 23:08:20 GMT  
		Size: 64.0 MB (63964214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a121fca9c95ea048128fa2a5b56995a6dc72e90529f4fa242e9f7c3e9b2cc56d`  
		Last Modified: Fri, 16 Dec 2022 01:02:51 GMT  
		Size: 59.6 MB (59600771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9c419e0f7da3b1d1e1ac9125a8c1f8eb36e88af7afecc880ac08af2ffa36f8`  
		Last Modified: Fri, 16 Dec 2022 01:25:21 GMT  
		Size: 3.6 MB (3633955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57f03c0548787b8df58aabedbc3fad39032bd6815d3568fca3666168e97e417`  
		Last Modified: Fri, 16 Dec 2022 01:25:21 GMT  
		Size: 8.7 MB (8739523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b65059dc2a8123b4e93282734870d204ffcd5789e099fc06ca714b789f2cad1`  
		Last Modified: Fri, 16 Dec 2022 01:25:21 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5970004bb9010109a79b6b8c2e1517c39882147e6326675b1fe822b9e1ae5411`  
		Last Modified: Fri, 16 Dec 2022 01:25:21 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
