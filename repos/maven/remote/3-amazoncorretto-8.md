## `maven:3-amazoncorretto-8`

```console
$ docker pull maven@sha256:384ebe341061b1e801c9f46d129f681ee777778a7b9d8a3296c2dd599817bcb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8` - linux; amd64

```console
$ docker pull maven@sha256:d5e394de2d8500816779e89db94b60977c40a91a150ad36fca9d3c916b82cffe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150392434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:721a12f2ac464ca9c1f63f07b00ab9ec811499df9221ef696c87ba6e6d777736`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 27 Jan 2021 22:19:43 GMT
ADD file:bcd0b903093ee2c81a54e8bdc50176f4038662ab936aa0d94af08458d508aef6 in / 
# Wed, 27 Jan 2021 22:19:43 GMT
CMD ["/bin/bash"]
# Wed, 27 Jan 2021 22:37:57 GMT
ARG version=1.8.0_282.b08-1
# Wed, 27 Jan 2021 22:38:12 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 27 Jan 2021 22:38:12 GMT
ENV LANG=C.UTF-8
# Wed, 27 Jan 2021 22:38:12 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 27 Jan 2021 22:58:10 GMT
ARG MAVEN_VERSION=3.6.3
# Wed, 27 Jan 2021 22:58:10 GMT
ARG USER_HOME_DIR=/root
# Wed, 27 Jan 2021 22:58:11 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Wed, 27 Jan 2021 22:58:11 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Wed, 27 Jan 2021 22:58:17 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 27 Jan 2021 22:58:21 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 27 Jan 2021 22:58:21 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 27 Jan 2021 22:58:21 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 27 Jan 2021 22:58:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 27 Jan 2021 22:58:21 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 27 Jan 2021 22:58:22 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 27 Jan 2021 22:58:22 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 27 Jan 2021 22:58:22 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:62350c28fdb7b7cbd0e199dd893555ed129ed85da482d882b1eeb574988ea7d6`  
		Last Modified: Wed, 27 Jan 2021 22:21:18 GMT  
		Size: 62.0 MB (61996576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ae5c605851bb4ddf423c11efa72971be53f62b857ebfa6067e07988ad95364`  
		Last Modified: Wed, 27 Jan 2021 22:39:58 GMT  
		Size: 75.3 MB (75270412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb07bba191559b8d989f0b517b110198d5fec53aca9e91099a7b44e3cdc44c`  
		Last Modified: Wed, 27 Jan 2021 23:00:25 GMT  
		Size: 3.5 MB (3543053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2d6da8d0e3a183c35e5ff17e1062e90e36f42894f9e36896165dfaceb71974`  
		Last Modified: Wed, 27 Jan 2021 23:00:25 GMT  
		Size: 9.6 MB (9581182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e11b31ba919f74c874862e0343928d243e477d73b41bdcb4cfd22ba497c8c8`  
		Last Modified: Wed, 27 Jan 2021 23:00:25 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c19bf9be7d8b80945eb68babad78b4e8f843665272d0184265ecdd5747c91ad`  
		Last Modified: Wed, 27 Jan 2021 23:00:25 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:fac5e7b612856d7429a10cce21d92e9bf4ea451e4759afb3f77ad4c266b99451
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136198942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c6bf3649db03b5a20733d1026c0386dd824743125e3a4ca6bc58ba05b7afd28`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 27 Jan 2021 23:09:56 GMT
ADD file:7f69686262e0e0e5415d42ac0371f7d0df0330bc4f0556e5d4b73dd78ceb1197 in / 
# Wed, 27 Jan 2021 23:10:02 GMT
CMD ["/bin/bash"]
# Wed, 27 Jan 2021 23:48:10 GMT
ARG version=1.8.0_282.b08-1
# Wed, 27 Jan 2021 23:48:39 GMT
# ARGS: version=1.8.0_282.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 27 Jan 2021 23:48:40 GMT
ENV LANG=C.UTF-8
# Wed, 27 Jan 2021 23:48:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Thu, 28 Jan 2021 00:26:07 GMT
ARG MAVEN_VERSION=3.6.3
# Thu, 28 Jan 2021 00:26:08 GMT
ARG USER_HOME_DIR=/root
# Thu, 28 Jan 2021 00:26:08 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Thu, 28 Jan 2021 00:26:09 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Thu, 28 Jan 2021 00:26:21 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Thu, 28 Jan 2021 00:26:25 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 28 Jan 2021 00:26:26 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 28 Jan 2021 00:26:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 28 Jan 2021 00:26:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Thu, 28 Jan 2021 00:26:28 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 28 Jan 2021 00:26:29 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 28 Jan 2021 00:26:30 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 28 Jan 2021 00:26:31 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:c6741bcf27a42820ff66e35cc842cec9a845e9e9dba4ff7bd465fc6161442a86`  
		Last Modified: Wed, 27 Jan 2021 23:11:10 GMT  
		Size: 63.7 MB (63704713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaab5df19070b49e0c6005600fe463b9dbdfeee6ccefc14abf2a5ffe3b8f64ad`  
		Last Modified: Wed, 27 Jan 2021 23:50:41 GMT  
		Size: 59.4 MB (59352471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c70647eaaf0198888c5d48ccfa3ba0a6aa7a427f03921ef7d20b77587627c30`  
		Last Modified: Thu, 28 Jan 2021 00:28:45 GMT  
		Size: 3.6 MB (3559330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe904df953ed2af5f32f73fee999ed7bd7fc557e684587b7efefbc71a96f9a07`  
		Last Modified: Thu, 28 Jan 2021 00:28:45 GMT  
		Size: 9.6 MB (9581216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033d9e69305ab3f04dc50258e9053622fc3e4501bd3bb05309cc2f691bb76119`  
		Last Modified: Thu, 28 Jan 2021 00:28:44 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44461f74dcb777fef4f0b160ce0a6f02143c1624214137ce8f856d1cfc9cfdb4`  
		Last Modified: Thu, 28 Jan 2021 00:28:44 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
