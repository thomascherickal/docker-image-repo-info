## `maven:3-amazoncorretto-17`

```console
$ docker pull maven@sha256:02af1d85d3cd514a6489e2bc1c35c9af826d02f92297fd1c505b66cafad30213
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17` - linux; amd64

```console
$ docker pull maven@sha256:f15b687c1082ebb86a446e5f99bffb48cc8449de2483afb13469cc8d2bbf438f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.2 MB (226196910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3d8523257530ace95eeac135ae2da5bd763fd73efb819c4689d9f665f42cf5`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 21 Oct 2021 22:19:45 GMT
ADD file:7aef897e53c30ca977c42dd7692208abbd381b7d2e7e07a91d929f3f0ac4ea5c in / 
# Thu, 21 Oct 2021 22:19:46 GMT
CMD ["/bin/bash"]
# Mon, 25 Oct 2021 18:24:03 GMT
ARG version=17.0.1.12-1
# Mon, 25 Oct 2021 18:24:26 GMT
# ARGS: version=17.0.1.12-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 25 Oct 2021 18:24:27 GMT
ENV LANG=C.UTF-8
# Mon, 25 Oct 2021 18:24:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Mon, 25 Oct 2021 19:10:08 GMT
ARG MAVEN_VERSION=3.8.3
# Mon, 25 Oct 2021 19:10:08 GMT
ARG USER_HOME_DIR=/root
# Mon, 25 Oct 2021 19:10:08 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Mon, 25 Oct 2021 19:10:08 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Mon, 25 Oct 2021 19:10:18 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Mon, 25 Oct 2021 19:10:27 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 25 Oct 2021 19:10:27 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 25 Oct 2021 19:10:27 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 25 Oct 2021 19:10:27 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 25 Oct 2021 19:10:28 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 25 Oct 2021 19:10:28 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 25 Oct 2021 19:10:28 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5263c4cb36ce7acd05658a221ec502b376a281d7a6075ad09beb23ac02a7668c`  
		Last Modified: Wed, 20 Oct 2021 18:03:24 GMT  
		Size: 62.0 MB (61976108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80f94f4a30a2bec83c6c2256573124c8dd3a24493fbdd6d14d65778f3172cc6`  
		Last Modified: Mon, 25 Oct 2021 18:27:05 GMT  
		Size: 151.5 MB (151524455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a44438c43220a5ea08a32533b515ffbb2ca8b5cfb0e36909fbd956479177db`  
		Last Modified: Mon, 25 Oct 2021 19:12:18 GMT  
		Size: 3.6 MB (3589497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210f19b1a675d7248c4ff712498c086763050f74a0d7a1984c15e68d25aecdca`  
		Last Modified: Mon, 25 Oct 2021 19:12:18 GMT  
		Size: 9.1 MB (9105638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55f1ee5aa9bd74298456cc70f65e2b2418ef42d51996e216ba0a2b8a7266862`  
		Last Modified: Mon, 25 Oct 2021 19:12:17 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf90eb447724c40d37df31e8ec2f72cba5210304de7d4e35b5b58d537aa1a62`  
		Last Modified: Mon, 25 Oct 2021 19:12:17 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:6b74303c7e5c1b64c623c6c891ad53310c42260d18426a5910bfeb2f016943a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226369726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45efb9fd9e78193421e5827dce0671f098860f21e3bafcb674deb0944f8c2b44`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 21 Oct 2021 21:39:54 GMT
ADD file:d9148106dadecc4050f37ebf22ea9e7e56102619349368d1ce40d36f5e2fadd1 in / 
# Thu, 21 Oct 2021 21:39:55 GMT
CMD ["/bin/bash"]
# Mon, 25 Oct 2021 17:39:36 GMT
ARG version=17.0.1.12-1
# Mon, 25 Oct 2021 17:39:55 GMT
# ARGS: version=17.0.1.12-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 25 Oct 2021 17:39:56 GMT
ENV LANG=C.UTF-8
# Mon, 25 Oct 2021 17:39:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Mon, 25 Oct 2021 18:04:17 GMT
ARG MAVEN_VERSION=3.8.3
# Mon, 25 Oct 2021 18:04:17 GMT
ARG USER_HOME_DIR=/root
# Mon, 25 Oct 2021 18:04:18 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Mon, 25 Oct 2021 18:04:19 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Mon, 25 Oct 2021 18:04:25 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Mon, 25 Oct 2021 18:04:44 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 25 Oct 2021 18:04:45 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 25 Oct 2021 18:04:46 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 25 Oct 2021 18:04:48 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 25 Oct 2021 18:04:49 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 25 Oct 2021 18:04:49 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 25 Oct 2021 18:04:50 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e20b44047a77430ceb5678bf23278ca2841835a1b18a72adaace3d3a11c56031`  
		Last Modified: Thu, 21 Oct 2021 21:40:44 GMT  
		Size: 63.6 MB (63606878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d478a1134542064a51c4342e71fea0cf27913748897bfcc5740a10fb2b93823`  
		Last Modified: Mon, 25 Oct 2021 17:41:14 GMT  
		Size: 150.0 MB (150046617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd30f28bf73d09bce57ccfe8d330aad2860deae3590146270dc80d576c5ab565`  
		Last Modified: Mon, 25 Oct 2021 18:07:43 GMT  
		Size: 3.6 MB (3609437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6624da5267c7aa230dc5e3baa30b15c97868df54ec7ffc757160476e4e3a6c`  
		Last Modified: Mon, 25 Oct 2021 18:07:43 GMT  
		Size: 9.1 MB (9105581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1749321ebbe7fa6730190cd46f42526dac8e1fb2a112fb68c3fcf8ae84264922`  
		Last Modified: Mon, 25 Oct 2021 18:07:42 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bc58c503d2a212a7702b75eb2aa1d9ed00d2f6489eeef0039e17695ea5421d`  
		Last Modified: Mon, 25 Oct 2021 18:07:42 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
