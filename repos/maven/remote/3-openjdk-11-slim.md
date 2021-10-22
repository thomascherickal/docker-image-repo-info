## `maven:3-openjdk-11-slim`

```console
$ docker pull maven@sha256:33082521e0afe3004a2b741bce032268a6f559b3cdb38a8089b74c8c552ac399
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-11-slim` - linux; amd64

```console
$ docker pull maven@sha256:9cbce68fb73e72f1db36c3daf7dd37a0548ba0ab3123a3a1fe5ef8fcf28bd6f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.9 MB (247896143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e1e6f6847f07206070e52b7644c9647b2d8f1611662a74e3d04817b93c8b907`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:27:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:32:52 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 12 Oct 2021 16:32:53 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 12 Oct 2021 16:32:54 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:32:54 GMT
ENV LANG=C.UTF-8
# Thu, 21 Oct 2021 23:44:06 GMT
ENV JAVA_VERSION=11.0.13
# Thu, 21 Oct 2021 23:44:26 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_linux_11.0.13_8.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_aarch64_linux_11.0.13_8.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 21 Oct 2021 23:44:27 GMT
CMD ["jshell"]
# Fri, 22 Oct 2021 00:06:57 GMT
ARG MAVEN_VERSION=3.8.3
# Fri, 22 Oct 2021 00:06:57 GMT
ARG USER_HOME_DIR=/root
# Fri, 22 Oct 2021 00:06:57 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Fri, 22 Oct 2021 00:06:57 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Fri, 22 Oct 2021 00:07:02 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN apt-get update &&     apt-get install -y       curl procps   && rm -rf /var/lib/apt/lists/*
# Fri, 22 Oct 2021 00:07:09 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 22 Oct 2021 00:07:09 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 22 Oct 2021 00:07:09 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 22 Oct 2021 00:07:10 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 22 Oct 2021 00:07:10 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 22 Oct 2021 00:07:10 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 22 Oct 2021 00:07:10 GMT
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
	-	`sha256:c78f8a9ed8840e88c8c3b0627b42a9405d360a5e44b32f2d7fe9a40e02329726`  
		Last Modified: Tue, 12 Oct 2021 16:50:55 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c9c563b3d60109cf873bc8a503e26a9f517264ae83e683b1faf40856116473`  
		Last Modified: Thu, 21 Oct 2021 23:59:08 GMT  
		Size: 203.4 MB (203391860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af25243e03f45338f7776eb1dbeec17d81084e713c3d48227ebd33566cbf94aa`  
		Last Modified: Fri, 22 Oct 2021 00:10:50 GMT  
		Size: 2.5 MB (2457870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fb27c20defb4ad309b58f51caf9e7c82d381d90f2e74df53c25f80bfbb35bf`  
		Last Modified: Fri, 22 Oct 2021 00:10:50 GMT  
		Size: 9.1 MB (9105635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7413fded1169bfccfa3701fefeb0d420536b0e0fb48697fee30a9d7cfe8295a`  
		Last Modified: Fri, 22 Oct 2021 00:10:49 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940f37f85322073c609653eabccc8ceb873368e5d4abf0d5b19d8bd51177fd58`  
		Last Modified: Fri, 22 Oct 2021 00:10:49 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-11-slim` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:1b0a42b3a3caef8a9b5b79cd4594e2953a6515b588ae8e9ce517323c5c20f245
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.8 MB (243763197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ed48b6043c1975728bd464fb6df9a54d35370fd5b64aa48fade3baf2e57d3b`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:18 GMT
ADD file:d84144ad575672cd6cc8a00c8e5a88ab0545348f040fc249ea5fcf8193b2bce6 in / 
# Tue, 12 Oct 2021 01:41:18 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 06:00:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 06:09:36 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 13 Oct 2021 06:09:37 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 13 Oct 2021 06:09:38 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 06:09:39 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 06:09:40 GMT
ENV JAVA_VERSION=11.0.12
# Wed, 13 Oct 2021 06:10:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 13 Oct 2021 06:10:01 GMT
CMD ["jshell"]
# Wed, 13 Oct 2021 08:00:55 GMT
ARG MAVEN_VERSION=3.8.3
# Wed, 13 Oct 2021 08:00:56 GMT
ARG USER_HOME_DIR=/root
# Wed, 13 Oct 2021 08:00:57 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Wed, 13 Oct 2021 08:00:58 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Wed, 13 Oct 2021 08:01:03 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN apt-get update &&     apt-get install -y       curl procps   && rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 08:01:09 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 13 Oct 2021 08:01:09 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 13 Oct 2021 08:01:10 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 13 Oct 2021 08:01:12 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 13 Oct 2021 08:01:13 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Wed, 13 Oct 2021 08:01:13 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 13 Oct 2021 08:01:14 GMT
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
	-	`sha256:f1c654db09bcc79500b8b4835083562086d498045750c7ce5721d4beab40690d`  
		Last Modified: Wed, 13 Oct 2021 06:38:41 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd0b847a9dac2a758f1ab28330b4694f5b66a33097d16a7508badbda901c6e0`  
		Last Modified: Wed, 13 Oct 2021 06:39:01 GMT  
		Size: 200.8 MB (200782689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62b280b1df71bfb77c3835adc9da6800aadbf03be288eb9384d6dc029ad216a`  
		Last Modified: Wed, 13 Oct 2021 08:18:33 GMT  
		Size: 2.3 MB (2263700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050a8f4fa8688fdd8f09f5a1cd5d648be9286a0b45e327b78cb604d9b0f2a1b9`  
		Last Modified: Wed, 13 Oct 2021 08:18:33 GMT  
		Size: 9.1 MB (9105568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425c9ba1e0c4fc1f1efefffa870810cc05905c88d4b9815f96c8939bf99e097d`  
		Last Modified: Wed, 13 Oct 2021 08:18:33 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b279b9c3d42ed51f6ba2cb86cab198f50dd90799f0cccd2d981e148b5c2fd3c`  
		Last Modified: Wed, 13 Oct 2021 08:18:33 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
