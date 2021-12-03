## `maven:3-amazoncorretto-17`

```console
$ docker pull maven@sha256:8e9405ae5720251d1fe275f85ff7e162a033ba5e4ec06ab63a282d32e51bd6f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17` - linux; amd64

```console
$ docker pull maven@sha256:f688f2f9c1ac387bade92e51fdbb4d3bd8d89c6d010a19fd29fb45b653f45c18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226370674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe46c5212f8773d48bc9167287832a255f8ab5e682feafa78d6f76b2b9a7f0c8`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 02 Dec 2021 23:20:03 GMT
ADD file:4eca58da351122eac20ffd87e3af2c0313089cb81650bdd4c2ef95a556fb842a in / 
# Thu, 02 Dec 2021 23:20:04 GMT
CMD ["/bin/bash"]
# Fri, 03 Dec 2021 21:52:54 GMT
ARG version=17.0.1.12-1
# Fri, 03 Dec 2021 21:53:16 GMT
# ARGS: version=17.0.1.12-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 03 Dec 2021 21:53:17 GMT
ENV LANG=C.UTF-8
# Fri, 03 Dec 2021 21:53:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Fri, 03 Dec 2021 22:54:42 GMT
ARG MAVEN_VERSION=3.8.4
# Fri, 03 Dec 2021 22:54:42 GMT
ARG USER_HOME_DIR=/root
# Fri, 03 Dec 2021 22:54:43 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Fri, 03 Dec 2021 22:54:43 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Fri, 03 Dec 2021 22:54:53 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 03 Dec 2021 22:54:55 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 03 Dec 2021 22:54:56 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 03 Dec 2021 22:54:56 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 03 Dec 2021 22:54:56 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 03 Dec 2021 22:54:56 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 03 Dec 2021 22:54:57 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 03 Dec 2021 22:54:57 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8b8a142162d22658bdf0283afcd00a9dd216c6637943ffe5f2ba53c4e3da0bd9`  
		Last Modified: Thu, 02 Dec 2021 06:01:08 GMT  
		Size: 62.1 MB (62090346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe03da6c601647ea7971247cde273c315f9a87637e184abace3a77b9e25464e`  
		Last Modified: Fri, 03 Dec 2021 21:56:17 GMT  
		Size: 151.5 MB (151540933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7c13e781bcfc3468ae127147eec4898ade7a0d88f368c3b4c8212176c1533e`  
		Last Modified: Fri, 03 Dec 2021 22:57:32 GMT  
		Size: 3.6 MB (3628379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d3252f7a3ace536442d04c220733c68f546b92bc2dc5d8fcb418c5d7731cf5`  
		Last Modified: Fri, 03 Dec 2021 22:57:32 GMT  
		Size: 9.1 MB (9109805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5455f17861b5b3668740e2aa0e93feaf5834d620eda8ff7408f78fa0c005c`  
		Last Modified: Fri, 03 Dec 2021 22:57:31 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0e84b295cc9844b0e3cc1a963e642f837db1dc97bdeb5531e3c2dad2193c98`  
		Last Modified: Fri, 03 Dec 2021 22:57:31 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:4d4f13485b20c03125ffcc21df0683d19e015112d3ca9a4aee16a6bba75a9e0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226448353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdec1ea160c96080a46af8641b0d41d5b869991c700acbc00044a39b9beec913`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 02 Dec 2021 21:25:17 GMT
ADD file:1f2ecfca149ab81a0527241077c1b366afd95b6b7a1dd91bddfd6c40988ba994 in / 
# Thu, 02 Dec 2021 21:25:18 GMT
CMD ["/bin/bash"]
# Fri, 03 Dec 2021 16:54:30 GMT
ARG version=17.0.1.12-1
# Fri, 03 Dec 2021 16:54:47 GMT
# ARGS: version=17.0.1.12-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 03 Dec 2021 16:54:47 GMT
ENV LANG=C.UTF-8
# Fri, 03 Dec 2021 16:54:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Fri, 03 Dec 2021 20:49:02 GMT
ARG MAVEN_VERSION=3.8.4
# Fri, 03 Dec 2021 20:49:03 GMT
ARG USER_HOME_DIR=/root
# Fri, 03 Dec 2021 20:49:04 GMT
ARG SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8
# Fri, 03 Dec 2021 20:49:05 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries
# Fri, 03 Dec 2021 20:49:10 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 03 Dec 2021 20:49:15 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.4/binaries MAVEN_VERSION=3.8.4 SHA=a9b2d825eacf2e771ed5d6b0e01398589ac1bfa4171f36154d1b5787879605507802f699da6f7cfc80732a5282fd31b28e4cd6052338cbef0fa1358b48a5e3c8 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 03 Dec 2021 20:49:15 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 03 Dec 2021 20:49:16 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 03 Dec 2021 20:49:18 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 03 Dec 2021 20:49:19 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 03 Dec 2021 20:49:19 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 03 Dec 2021 20:49:20 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:74f9a6be36f3bc3bf6041c40376d548e3a8b720a0455674b19e9174a9e567078`  
		Last Modified: Thu, 02 Dec 2021 21:26:12 GMT  
		Size: 63.7 MB (63692547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca22289d3bc8d639ce9c21bc5edc611c4a87f936cdb6557abb4af42a1d431143`  
		Last Modified: Fri, 03 Dec 2021 16:56:46 GMT  
		Size: 150.1 MB (150051510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabafffd24c1190526c30c5e0b213f6dcd43668a0b4abc0094f7e724e531c088`  
		Last Modified: Fri, 03 Dec 2021 20:52:51 GMT  
		Size: 3.6 MB (3593307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffbb8892512a8c0dbbee15c5db7a314aef4bf70de8e310e5d036ca31494ab2e`  
		Last Modified: Fri, 03 Dec 2021 20:52:51 GMT  
		Size: 9.1 MB (9109777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b1faf74aeb3133aa1dbb9fb5f4713f4dd947e630a8f004dc90782ed3fb5064`  
		Last Modified: Fri, 03 Dec 2021 20:52:50 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6842eb3d11733fcfe8f56c8fa9cb88eee2e3cb445258bea7fc60b8febc4a5c23`  
		Last Modified: Fri, 03 Dec 2021 20:52:50 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
