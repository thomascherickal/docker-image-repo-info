## `maven:3-amazoncorretto-8`

```console
$ docker pull maven@sha256:5856d35051a0715899b2d2dc98449567d8937940b0e62b83fa6ba5ecd22d47b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8` - linux; amd64

```console
$ docker pull maven@sha256:3b61f0b5af2ebf64454a43f1405c59dc287048d3e8f35390fc8cea34afd10032
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.3 MB (150260686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8732570bef447dd6621ca2259b5179dde7dcd908c6c142890ce6ac60b2d03b09`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 12 Aug 2022 00:20:15 GMT
ADD file:56a385790046ac5dfb85932009eb1e99c8593221e306b937274c477c05cc9886 in / 
# Fri, 12 Aug 2022 00:20:15 GMT
CMD ["/bin/bash"]
# Fri, 12 Aug 2022 02:59:13 GMT
ARG version=1.8.0_342.b07-4
# Fri, 12 Aug 2022 02:59:39 GMT
# ARGS: version=1.8.0_342.b07-4
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 12 Aug 2022 02:59:39 GMT
ENV LANG=C.UTF-8
# Fri, 12 Aug 2022 02:59:40 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 12 Aug 2022 04:15:09 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 12 Aug 2022 04:15:09 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 12 Aug 2022 04:15:09 GMT
ARG USER_HOME_DIR=/root
# Fri, 12 Aug 2022 04:15:10 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 12 Aug 2022 04:15:10 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 12 Aug 2022 04:15:11 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 12 Aug 2022 04:15:12 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 12 Aug 2022 04:15:12 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 12 Aug 2022 04:15:12 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 12 Aug 2022 04:15:12 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 12 Aug 2022 04:15:12 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 12 Aug 2022 04:15:12 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 12 Aug 2022 04:15:12 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5e0be87f98fb0e8a6ecddb6b717178ddc6555638e6e89d39929d47654b79739d`  
		Last Modified: Mon, 01 Aug 2022 22:09:03 GMT  
		Size: 62.3 MB (62316216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2ed3f8d08aa74e8f95ecdbb438976bc6be9725b4cfd8226c0951916bad35f2`  
		Last Modified: Fri, 12 Aug 2022 03:03:40 GMT  
		Size: 75.6 MB (75573752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3624505671e77b9757a8ac39c82052ed0b6d679abbe472209a97fa1b666cf0e6`  
		Last Modified: Fri, 12 Aug 2022 04:17:39 GMT  
		Size: 3.6 MB (3630001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14475c36265b162a62a5e3516c229e4b08aebc9c6f83eae58c4ad01e0d326c41`  
		Last Modified: Fri, 12 Aug 2022 04:17:39 GMT  
		Size: 8.7 MB (8739501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d404139306e59c00a64184b816e131d7d9178929b8a05bab5fd794961ee529fc`  
		Last Modified: Fri, 12 Aug 2022 04:17:39 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0ba330b0d124d5d719e7d95faab5a7c34676af7fc60c11c5913dbe2849b56a`  
		Last Modified: Fri, 12 Aug 2022 04:17:39 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:8ae719b5307274c092f0998eb753b4b4efbd90a36c0ac1f647d1ec41f00785f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.9 MB (135893544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4662b886193f4c1b90a43e9729a8d7e1ef24c2100f4f36f583ad47384a880d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 21 Jun 2022 23:39:32 GMT
ADD file:ce3840583311a5848d47c22463b3a966c40bbf4824f1c9b9b2c51e2fb939de3a in / 
# Tue, 21 Jun 2022 23:39:33 GMT
CMD ["/bin/bash"]
# Fri, 29 Jul 2022 19:39:24 GMT
ARG version=1.8.0_342.b07-4
# Fri, 29 Jul 2022 19:39:39 GMT
# ARGS: version=1.8.0_342.b07-4
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 29 Jul 2022 19:39:39 GMT
ENV LANG=C.UTF-8
# Fri, 29 Jul 2022 19:39:40 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 29 Jul 2022 20:08:17 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 29 Jul 2022 20:08:18 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 29 Jul 2022 20:08:19 GMT
ARG USER_HOME_DIR=/root
# Fri, 29 Jul 2022 20:08:20 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 29 Jul 2022 20:08:21 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 29 Jul 2022 20:08:29 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 29 Jul 2022 20:08:30 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 29 Jul 2022 20:08:31 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 29 Jul 2022 20:08:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 29 Jul 2022 20:08:34 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 29 Jul 2022 20:08:35 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 29 Jul 2022 20:08:35 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 29 Jul 2022 20:08:36 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8cd18ebacb4abd924911c002d3ec5b8d76247c7ed5fff822c8cfb3961846f05a`  
		Last Modified: Wed, 15 Jun 2022 22:09:35 GMT  
		Size: 63.9 MB (63918642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8f60aacf01af6baad600fbdc1827a45e57f77af3ecffb101b18e8231622bdb`  
		Last Modified: Fri, 29 Jul 2022 19:40:52 GMT  
		Size: 59.6 MB (59602385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7909d9859491e6e9026ac1d2e71650f5e3056d596c75b695aa61749dc14ba0`  
		Last Modified: Fri, 29 Jul 2022 20:12:05 GMT  
		Size: 3.6 MB (3631821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11368750761c447844e56c94c4b389080c0fc17c51d000d9e59f0dcc5ffe2fa4`  
		Last Modified: Fri, 29 Jul 2022 20:12:05 GMT  
		Size: 8.7 MB (8739479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9c21a40b71f59ffa2e7cba8c2f7e556f4cfee00228d026c4a6ca0467c77604`  
		Last Modified: Fri, 29 Jul 2022 20:12:04 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7f3d0175c9ae56b28f6d859750e22ecf9e2b0f63092ddec927ac2a4d890edb`  
		Last Modified: Fri, 29 Jul 2022 20:12:04 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
