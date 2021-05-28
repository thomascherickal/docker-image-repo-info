## `maven:3-amazoncorretto`

```console
$ docker pull maven@sha256:6025fc02724d64e224497c3b675ab317679e564b4f2919525dc7c2f57b1d667d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto` - linux; amd64

```console
$ docker pull maven@sha256:89a977292d9f7f7373b64d2f0793e671f270d5275312ace0cf829a1559ba7999
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.8 MB (221820801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e79b69cfca1d243e9f1c01c886450b816f904b34a03388cb39bada40445d48c9`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 29 Apr 2021 22:25:37 GMT
ADD file:47fcf0318dccec16b61a0d21a0f16c45b77dea5abf50ba6604f1ffadcb299d10 in / 
# Thu, 29 Apr 2021 22:25:38 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:44:48 GMT
ARG version=11.0.11.9-1
# Thu, 29 Apr 2021 22:45:13 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 29 Apr 2021 22:45:13 GMT
ENV LANG=C.UTF-8
# Thu, 29 Apr 2021 22:45:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Thu, 29 Apr 2021 23:12:35 GMT
ARG MAVEN_VERSION=3.8.1
# Thu, 29 Apr 2021 23:12:35 GMT
ARG USER_HOME_DIR=/root
# Thu, 29 Apr 2021 23:12:35 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Thu, 29 Apr 2021 23:12:35 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Thu, 29 Apr 2021 23:12:45 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Thu, 29 Apr 2021 23:12:47 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 29 Apr 2021 23:12:48 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 29 Apr 2021 23:12:48 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 29 Apr 2021 23:12:48 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 29 Apr 2021 23:12:48 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 29 Apr 2021 23:12:48 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 29 Apr 2021 23:12:48 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3c2c91c7c4311eca863331479504040ee4f45fda9a610947b82886e7bbd5b737`  
		Last Modified: Thu, 29 Apr 2021 22:27:18 GMT  
		Size: 61.9 MB (61947132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17eb3d153b3376801c1da7fc410637e77e5b7e2891bf6e58d32dc6a02ab1473a`  
		Last Modified: Thu, 29 Apr 2021 22:47:15 GMT  
		Size: 146.7 MB (146668563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179994bcd834bdfde319f4ea4cbdf4cf836ab62bca89025b19bee3f639bcc35f`  
		Last Modified: Thu, 29 Apr 2021 23:15:39 GMT  
		Size: 3.6 MB (3592934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16ff32b04d5e5fa321b6be59805d02e9227eefb2d497344a3a5a24d9123f566`  
		Last Modified: Thu, 29 Apr 2021 23:15:39 GMT  
		Size: 9.6 MB (9610963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c234d73ccfcad32f2217017cda7c8445e4ae7b81351a9efa546b98e1a64267f`  
		Last Modified: Thu, 29 Apr 2021 23:15:38 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8186dfe8f88b53d295e4bb834ef088d5f2e2a9a54e47fb961a488a39aa8dd82c`  
		Last Modified: Thu, 29 Apr 2021 23:15:38 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:6fa9a18668d8e907f36f43a4d80d595fb05e0c78c7e81d9d05b886f121530748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.6 MB (221603812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c69e2d6659a73032b812e90ab1c159c4a057579017b9851bb52258877d574527`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 29 Apr 2021 22:40:32 GMT
ADD file:03605b69274d89b78234df03d53dacc9cac408d68b82b1fb5d63b84c01b69300 in / 
# Thu, 29 Apr 2021 22:40:37 GMT
CMD ["/bin/bash"]
# Fri, 28 May 2021 12:43:40 GMT
ARG version=11.0.11.9-1
# Fri, 28 May 2021 12:44:04 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 28 May 2021 12:44:05 GMT
ENV LANG=C.UTF-8
# Fri, 28 May 2021 12:44:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Fri, 28 May 2021 14:12:33 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 28 May 2021 14:12:33 GMT
ARG USER_HOME_DIR=/root
# Fri, 28 May 2021 14:12:33 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 28 May 2021 14:12:33 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 28 May 2021 14:12:42 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 28 May 2021 14:12:44 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 28 May 2021 14:12:44 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 28 May 2021 14:12:44 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 28 May 2021 14:12:44 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 28 May 2021 14:12:44 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 28 May 2021 14:12:45 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 28 May 2021 14:12:45 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:316be4ce82c0add9f71a6ce1face38b99f456abd45232cf7ad96ccac098ef5fe`  
		Last Modified: Thu, 29 Apr 2021 22:41:52 GMT  
		Size: 63.7 MB (63660068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282e067ed9fb0b1d0ac7eeba2ed63d75475e0a7372a956784b5c4ebb52e26077`  
		Last Modified: Fri, 28 May 2021 12:46:08 GMT  
		Size: 144.7 MB (144746416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12af54b425b9d2c36a8ff498f6c9ecd4cebf158479ce38edd55cf1a9e5dcf4ee`  
		Last Modified: Fri, 28 May 2021 14:19:46 GMT  
		Size: 3.6 MB (3585142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19db97c9fa15798d82322b1f6dc79d6bf7c069820829e9a74c81813ee9046b9d`  
		Last Modified: Fri, 28 May 2021 14:19:45 GMT  
		Size: 9.6 MB (9610974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba994297ad5a5d13c3b9b0eb760fd0d4c948f1a8abbe948eb09b31105562ab6`  
		Last Modified: Fri, 28 May 2021 14:19:44 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c42c400b3ec581b8784f4f1c3ff82db4e67f7e4c5bf8c06a314bee106e4a41`  
		Last Modified: Fri, 28 May 2021 14:19:44 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
