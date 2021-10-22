## `maven:amazoncorretto`

```console
$ docker pull maven@sha256:7ceaaca7b43d881631f021c5d52392f15792679478b89dd7bc9d4160f8656bbb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:amazoncorretto` - linux; amd64

```console
$ docker pull maven@sha256:4a4e87fb314e607438bd9b7608e1a34f4b2973e164282b65848ebe2f23ba574e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221453282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2ac42c0b9cace4ee595435b2ebf292ec7c44c6285032ebc156b278247d21847`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 21 Oct 2021 22:19:45 GMT
ADD file:7aef897e53c30ca977c42dd7692208abbd381b7d2e7e07a91d929f3f0ac4ea5c in / 
# Thu, 21 Oct 2021 22:19:46 GMT
CMD ["/bin/bash"]
# Thu, 21 Oct 2021 23:28:10 GMT
ARG version=11.0.13.8-1
# Thu, 21 Oct 2021 23:28:33 GMT
# ARGS: version=11.0.13.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 21 Oct 2021 23:28:34 GMT
ENV LANG=C.UTF-8
# Thu, 21 Oct 2021 23:28:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Fri, 22 Oct 2021 00:07:50 GMT
ARG MAVEN_VERSION=3.8.3
# Fri, 22 Oct 2021 00:07:50 GMT
ARG USER_HOME_DIR=/root
# Fri, 22 Oct 2021 00:07:50 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Fri, 22 Oct 2021 00:07:50 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Fri, 22 Oct 2021 00:08:00 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 22 Oct 2021 00:08:07 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 22 Oct 2021 00:08:07 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 22 Oct 2021 00:08:07 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 22 Oct 2021 00:08:07 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 22 Oct 2021 00:08:07 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 22 Oct 2021 00:08:08 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 22 Oct 2021 00:08:08 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5263c4cb36ce7acd05658a221ec502b376a281d7a6075ad09beb23ac02a7668c`  
		Last Modified: Wed, 20 Oct 2021 18:03:24 GMT  
		Size: 62.0 MB (61976108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9fa85bea77510327bc7908e11b491f6298bdc25fab855d9265928c2f0a9283`  
		Last Modified: Thu, 21 Oct 2021 23:32:02 GMT  
		Size: 146.8 MB (146770732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b41a30bca5690098db9cad4ef82ee999fa9289ae5b714a9b156f498e23e9d1`  
		Last Modified: Fri, 22 Oct 2021 00:12:12 GMT  
		Size: 3.6 MB (3599599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c962c1cc327a012e962e60442c4709a9e78f69a77be011e4fae2ce949e0c82`  
		Last Modified: Fri, 22 Oct 2021 00:12:12 GMT  
		Size: 9.1 MB (9105633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a9b94aea90c9362f85c9265ce4d33368915985d97166b73cf60852dcc60e45`  
		Last Modified: Fri, 22 Oct 2021 00:12:11 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57e985d0d704b8b7a6b7e530fd751886aa2527b5ddfc25eb07e7a8f7ffe1d7d`  
		Last Modified: Fri, 22 Oct 2021 00:12:11 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:4c090344cc5bab26883f1129e84485d8ea1428b945f0d15b6f2aa47144c4c917
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.2 MB (220218223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e99a8b766be066204ced4d04c7967e98c570d1ee4027696940477ad0dba64c4b`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 01 Oct 2021 21:39:54 GMT
ADD file:1d2ae2bfc4c1f83dc53f48b42503812d345622ab95d8fc84536216ef3d53d807 in / 
# Fri, 01 Oct 2021 21:39:55 GMT
CMD ["/bin/bash"]
# Wed, 20 Oct 2021 18:39:48 GMT
ARG version=11.0.13.8-1
# Wed, 20 Oct 2021 18:40:05 GMT
# ARGS: version=11.0.13.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 20 Oct 2021 18:40:06 GMT
ENV LANG=C.UTF-8
# Wed, 20 Oct 2021 18:40:06 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Wed, 20 Oct 2021 20:43:06 GMT
ARG MAVEN_VERSION=3.8.3
# Wed, 20 Oct 2021 20:43:07 GMT
ARG USER_HOME_DIR=/root
# Wed, 20 Oct 2021 20:43:08 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Wed, 20 Oct 2021 20:43:09 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Wed, 20 Oct 2021 20:43:15 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 20 Oct 2021 20:43:31 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 20 Oct 2021 20:43:31 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 20 Oct 2021 20:43:32 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 20 Oct 2021 20:43:34 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 20 Oct 2021 20:43:35 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 20 Oct 2021 20:43:35 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 20 Oct 2021 20:43:36 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5aa4871be3ec1bcadf7a5257231adc7740edac9a612749884f03ab14b4b2d4ec`  
		Last Modified: Fri, 01 Oct 2021 16:32:04 GMT  
		Size: 63.6 MB (63581978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f86063a188a1eb8ae4745dfab1e885f41d5d942def8b15d330a87992b364360`  
		Last Modified: Wed, 20 Oct 2021 18:42:28 GMT  
		Size: 143.9 MB (143922526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9110461b6ca96f321c01b280f55b4dc2e9adafbfbbf8368e6743633504da89b5`  
		Last Modified: Wed, 20 Oct 2021 20:48:43 GMT  
		Size: 3.6 MB (3606925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf74fcde9f066bfd9c88b0520e2ec51a54c229338938cff66ae554661ce7c47`  
		Last Modified: Wed, 20 Oct 2021 20:48:43 GMT  
		Size: 9.1 MB (9105580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b557f68762588acdba74f3678dc0d09f61b5b817f66ce6e33b73f20e1e163ae`  
		Last Modified: Wed, 20 Oct 2021 20:48:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0aa3e5d334ded93966d145fb1619db2e0a1fc2c6367e33f1f27bf9af4ab06`  
		Last Modified: Wed, 20 Oct 2021 20:48:42 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
