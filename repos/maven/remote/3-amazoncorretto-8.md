## `maven:3-amazoncorretto-8`

```console
$ docker pull maven@sha256:aa6174913009b0370607c0b276f557a14e58386957cf33117a80d0c4d8194dd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8` - linux; amd64

```console
$ docker pull maven@sha256:7da5c089c1e65792aa1032ba51cc49917bae7133b2acdaf3757d96fd2efd7e5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.0 MB (150001941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4aea6e41f903800ff4675adc5f8144aac2a9042b0bc76552593a44fe19713bb`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 01 Oct 2021 21:20:20 GMT
ADD file:21dc1ad70daefae1cf0e1b3e78fab06decda5cb9bc958d8a178adb3eddd1fb32 in / 
# Fri, 01 Oct 2021 21:20:20 GMT
CMD ["/bin/bash"]
# Fri, 01 Oct 2021 21:39:00 GMT
ARG version=1.8.0_302.b08-1
# Fri, 01 Oct 2021 21:39:20 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 01 Oct 2021 21:39:20 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 21:39:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 06 Oct 2021 21:16:55 GMT
ARG MAVEN_VERSION=3.8.3
# Wed, 06 Oct 2021 21:16:55 GMT
ARG USER_HOME_DIR=/root
# Wed, 06 Oct 2021 21:16:55 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Wed, 06 Oct 2021 21:16:55 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Wed, 06 Oct 2021 21:17:05 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 06 Oct 2021 21:17:07 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 06 Oct 2021 21:17:07 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 06 Oct 2021 21:17:07 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 06 Oct 2021 21:17:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 06 Oct 2021 21:17:08 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 06 Oct 2021 21:17:08 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 06 Oct 2021 21:17:08 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 06 Oct 2021 21:17:08 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:0728ce74490afacced1ac863ee989913071f97c52ab996e46cdd6b5369a2d63a`  
		Last Modified: Fri, 01 Oct 2021 10:54:14 GMT  
		Size: 62.0 MB (61952638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4427fc41f60de7402bd4220fcc04d95ec47eca25a9d36918efdf2beae74a0bdd`  
		Last Modified: Fri, 01 Oct 2021 21:41:47 GMT  
		Size: 75.3 MB (75341685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05680489438ecfef359c868dc2cbfb569cb4eba062db77fd88330be15cfb04e0`  
		Last Modified: Wed, 06 Oct 2021 21:27:51 GMT  
		Size: 3.6 MB (3600775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5cfff5fbc32447040781e8f5842a320471e0a543a7c2d3208206538d1f92fd`  
		Last Modified: Wed, 06 Oct 2021 21:27:51 GMT  
		Size: 9.1 MB (9105630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b6cf34b40f6178b0386c902add00b41ace789b83e7eea88315e86469afa845`  
		Last Modified: Wed, 06 Oct 2021 21:27:50 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc3bda95b00fc56ea9c3d911d0b01c994fd42d32e19c200ed9a08a629c096f7`  
		Last Modified: Wed, 06 Oct 2021 21:27:50 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:1c217d686ebd67a4914a6e2cf2d9f26029261e0fc63014f2de6b87430c076c29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135667668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67631a9350532abe19f5e02f7acd2774204ba68df7f44180c1d800553e183c27`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 01 Oct 2021 21:39:54 GMT
ADD file:1d2ae2bfc4c1f83dc53f48b42503812d345622ab95d8fc84536216ef3d53d807 in / 
# Fri, 01 Oct 2021 21:39:55 GMT
CMD ["/bin/bash"]
# Fri, 01 Oct 2021 21:57:32 GMT
ARG version=1.8.0_302.b08-1
# Fri, 01 Oct 2021 21:57:50 GMT
# ARGS: version=1.8.0_302.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 01 Oct 2021 21:57:50 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 21:57:50 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 06 Oct 2021 21:23:15 GMT
ARG MAVEN_VERSION=3.8.3
# Wed, 06 Oct 2021 21:23:15 GMT
ARG USER_HOME_DIR=/root
# Wed, 06 Oct 2021 21:23:15 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Wed, 06 Oct 2021 21:23:16 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Wed, 06 Oct 2021 21:23:23 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Wed, 06 Oct 2021 21:23:29 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 06 Oct 2021 21:23:30 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 06 Oct 2021 21:23:30 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 06 Oct 2021 21:23:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 06 Oct 2021 21:23:30 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 06 Oct 2021 21:23:30 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 06 Oct 2021 21:23:30 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 06 Oct 2021 21:23:31 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5aa4871be3ec1bcadf7a5257231adc7740edac9a612749884f03ab14b4b2d4ec`  
		Last Modified: Fri, 01 Oct 2021 16:32:04 GMT  
		Size: 63.6 MB (63581978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59aa11c1c46065f0e96c13fcd24b5d373b0d7152e74ec2eaa61aa3c0582ede4`  
		Last Modified: Fri, 01 Oct 2021 22:00:20 GMT  
		Size: 59.4 MB (59393641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3537a1a1662a7e6fffc927c47df699faad5251f518a186c9b9b39ebea302f631`  
		Last Modified: Wed, 06 Oct 2021 21:34:50 GMT  
		Size: 3.6 MB (3585200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75c2d144a4039c7c4751a1eb6b5f510a89d594d096e53e48c647efed12807d8`  
		Last Modified: Wed, 06 Oct 2021 21:34:50 GMT  
		Size: 9.1 MB (9105637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641d44c70e2dad501f8ccba3ee25e27ac39348b65618b31f0fc2d859f62931dd`  
		Last Modified: Wed, 06 Oct 2021 21:34:49 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44365e8e4a18f670e31c80835d39ecd9542e8d27d9d49827e97249637e6c7054`  
		Last Modified: Wed, 06 Oct 2021 21:34:49 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
