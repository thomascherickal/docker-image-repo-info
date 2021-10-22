## `maven:3-openjdk-8-slim`

```console
$ docker pull maven@sha256:090abd9aaa88c976603ab20c83e9a178a8c75daf9707f3bf98a54d72e7427274
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-8-slim` - linux; amd64

```console
$ docker pull maven@sha256:732c2669811c77f2f2ecc7695a614d48ca1ba2fcabecaa09d96546481965c8c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.8 MB (150775423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e88a961552211e6d5b81dfd313010fef82cdb814f138fb4f706e76a536b691a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:27:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:35:53 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 12 Oct 2021 16:35:54 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 12 Oct 2021 16:35:54 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:35:54 GMT
ENV LANG=C.UTF-8
# Thu, 21 Oct 2021 23:47:04 GMT
ENV JAVA_VERSION=8u312
# Thu, 21 Oct 2021 23:47:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 22 Oct 2021 00:07:20 GMT
ARG MAVEN_VERSION=3.8.3
# Fri, 22 Oct 2021 00:07:20 GMT
ARG USER_HOME_DIR=/root
# Fri, 22 Oct 2021 00:07:20 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Fri, 22 Oct 2021 00:07:21 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Fri, 22 Oct 2021 00:07:25 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN apt-get update &&     apt-get install -y       curl procps   && rm -rf /var/lib/apt/lists/*
# Fri, 22 Oct 2021 00:07:28 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 22 Oct 2021 00:07:28 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 22 Oct 2021 00:07:28 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 22 Oct 2021 00:07:28 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 22 Oct 2021 00:07:28 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 22 Oct 2021 00:07:29 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 22 Oct 2021 00:07:29 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225be9814eda07dabebf0e4deb415366f34b2cfe12ef1ad167ba1104423f42d7`  
		Last Modified: Tue, 12 Oct 2021 16:42:59 GMT  
		Size: 1.6 MB (1582043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76abba36541d6e4db03072637afec3ed62ce29f01f72d9f3d0d82801e2ccafb0`  
		Last Modified: Tue, 12 Oct 2021 16:54:55 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92736b03e888d05efe5691431c5108670cc4d967d6d4ab47babed607c6aed1b3`  
		Last Modified: Fri, 22 Oct 2021 00:03:43 GMT  
		Size: 106.3 MB (106272164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53eaa6d2ba10da1175a1f8a09642deb596dd4e3f8e6127652816d2b3b1395a8e`  
		Last Modified: Fri, 22 Oct 2021 00:11:33 GMT  
		Size: 2.5 MB (2456840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3d90806329c26eb699d2abaa961d84eb5e08c52af721e6d0d3e4e19f41a2eb`  
		Last Modified: Fri, 22 Oct 2021 00:11:33 GMT  
		Size: 9.1 MB (9105638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:900f68e26647983698e57bb30ca3192efc9c52e39e0eb3145029d0f9ea432561`  
		Last Modified: Fri, 22 Oct 2021 00:11:32 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7e46ba91bc315b5c2622eebe9a1683261e0db69487fdafccb0df018295e69a`  
		Last Modified: Fri, 22 Oct 2021 00:11:33 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-8-slim` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:8317caf37121acd85df897221b5ebc1b5db9627fd6ab041f015063e94186310a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.0 MB (148034902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a03317b8e875570f5996d40d5c91d667206bdf9cef9531121ef769174d1933a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:18 GMT
ADD file:d84144ad575672cd6cc8a00c8e5a88ab0545348f040fc249ea5fcf8193b2bce6 in / 
# Tue, 12 Oct 2021 01:41:18 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 06:00:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:14:00 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 13 Oct 2021 06:14:01 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 13 Oct 2021 06:14:02 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 06:14:03 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 06:14:04 GMT
ENV JAVA_VERSION=8u302
# Wed, 13 Oct 2021 06:14:18 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Wed, 13 Oct 2021 08:04:04 GMT
ARG MAVEN_VERSION=3.8.3
# Wed, 13 Oct 2021 08:04:05 GMT
ARG USER_HOME_DIR=/root
# Wed, 13 Oct 2021 08:04:06 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Wed, 13 Oct 2021 08:04:07 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Wed, 13 Oct 2021 08:04:12 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN apt-get update &&     apt-get install -y       curl procps   && rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 08:04:31 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 13 Oct 2021 08:04:31 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 13 Oct 2021 08:04:32 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 13 Oct 2021 08:04:34 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 13 Oct 2021 08:04:35 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 13 Oct 2021 08:04:35 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 13 Oct 2021 08:04:36 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a9eb63951c1c2ee8efcc12b696928fee3741a2d4eae76f2da3e161a5d90548bf`  
		Last Modified: Tue, 12 Oct 2021 01:48:13 GMT  
		Size: 30.0 MB (30043906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8552e0d309d6deaf17b87f395ca03a5bb0b4c14128cd49208ab21c34bf39e933`  
		Last Modified: Wed, 13 Oct 2021 06:25:32 GMT  
		Size: 1.6 MB (1565908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56792fb4f05d3842379b98d3522c4935555806215e308ecdfd3e8a195bd4c39`  
		Last Modified: Wed, 13 Oct 2021 06:44:03 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db1d11e583748fb40722ee375672fa4f2063015e8b5ea638f9981db8954bea3`  
		Last Modified: Wed, 13 Oct 2021 06:44:14 GMT  
		Size: 105.1 MB (105055827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196ea21495cf7cfe2a441f5c134f22f186e624a3865d069ba6780bb717352d8f`  
		Last Modified: Wed, 13 Oct 2021 08:19:23 GMT  
		Size: 2.3 MB (2262258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaad8b656388d6b4413095bce20127a1f348c38e1ba32397f79249d8939fc3a`  
		Last Modified: Wed, 13 Oct 2021 08:19:23 GMT  
		Size: 9.1 MB (9105571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c2fb23627eec86d99dc5dfc13a514e79ff972bfa26cf2db88e02e8a8987192`  
		Last Modified: Wed, 13 Oct 2021 08:19:22 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6e64dd41b0dbe1e91a4876ec380b15d3e6a0447e179fab820f226b0f383f1e`  
		Last Modified: Wed, 13 Oct 2021 08:19:22 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
