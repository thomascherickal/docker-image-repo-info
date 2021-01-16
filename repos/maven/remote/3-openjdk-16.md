## `maven:3-openjdk-16`

```console
$ docker pull maven@sha256:82d66d44feafab72ff7a9d0c7215053ccd013616f0b2b9986b1a8e7bb2a5d51d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-16` - linux; amd64

```console
$ docker pull maven@sha256:0e0d2e6f2836905ace6bb6ddf566ea51dd0bd90eb32d7cb01f7b2af850958ead
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **389.0 MB (389007681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c7c15d3a419a95bb3ae3f2f871a912484d1951b2f850fbdd782a773e4896574`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 15 Jan 2021 00:30:38 GMT
ADD file:2987f8143a9c4f758731c17e307a6c7ca9e5e1a974df3405a17d2699da7d8351 in / 
# Fri, 15 Jan 2021 00:30:39 GMT
CMD ["/bin/bash"]
# Fri, 15 Jan 2021 00:56:52 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 15 Jan 2021 00:56:53 GMT
ENV LANG=C.UTF-8
# Fri, 15 Jan 2021 00:59:09 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 15 Jan 2021 00:59:09 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Jan 2021 23:22:34 GMT
ENV JAVA_VERSION=16-ea+32
# Fri, 15 Jan 2021 23:23:30 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/32/GPL/openjdk-16-ea+32_linux-aarch64_bin.tar.gz; 			downloadSha256=c4ccb6df63b7b973504ad4dec0164d308d5dce7a5e2dcc508180deda33d4e61a; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/32/GPL/openjdk-16-ea+32_linux-x64_bin.tar.gz; 			downloadSha256=c951c0f2d55bc67fecbe0913675811721d13de16f4a81bf5363b660d17c02f0b; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 15 Jan 2021 23:23:30 GMT
CMD ["jshell"]
# Sat, 16 Jan 2021 01:43:00 GMT
ARG MAVEN_VERSION=3.6.3
# Sat, 16 Jan 2021 01:43:01 GMT
ARG USER_HOME_DIR=/root
# Sat, 16 Jan 2021 01:43:01 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Sat, 16 Jan 2021 01:43:01 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Sat, 16 Jan 2021 01:43:29 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN microdnf install findutils git
# Sat, 16 Jan 2021 01:43:33 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 16 Jan 2021 01:43:33 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 16 Jan 2021 01:43:33 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 16 Jan 2021 01:43:33 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 16 Jan 2021 01:43:34 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 16 Jan 2021 01:43:34 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 16 Jan 2021 01:43:34 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a73adebe9317092fb1f120a1d0d21f460296e9bde7ac683fd452cfc628c528cf`  
		Last Modified: Wed, 06 Jan 2021 20:23:26 GMT  
		Size: 42.1 MB (42069921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73bcd34cfec7fc27d7cd00bc22af06df0471526a6d2ceb8e77391a82f300f0`  
		Last Modified: Fri, 15 Jan 2021 01:08:29 GMT  
		Size: 13.3 MB (13277589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205463ba637e084f29b4052ae4482aa4ae29881e39f46dd0b5b17dd1f7581fb2`  
		Last Modified: Fri, 15 Jan 2021 23:35:30 GMT  
		Size: 184.8 MB (184751620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5f854bd1dcf1ba683c5bdf95c0140a000459e91fbc2be871bb4cfb776245d9`  
		Last Modified: Sat, 16 Jan 2021 01:46:58 GMT  
		Size: 139.3 MB (139326117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfeab3474fd72ddcc20c7bdd51f8170b97b94227a20a499b3e72a00f1560060`  
		Last Modified: Sat, 16 Jan 2021 01:46:44 GMT  
		Size: 9.6 MB (9581217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4011ed1ebb83c4b44776a7e9fde6040dcd26d8f9e085da04a2399a76c9bf76ad`  
		Last Modified: Sat, 16 Jan 2021 01:46:42 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abb645a2aa8e165c0bfed18263d1a3ff9f0cedddc307371bd9f0cf56f5201ae`  
		Last Modified: Sat, 16 Jan 2021 01:46:46 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-16` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:1d94643cd0dc93f227553ad43e685cc2188ee91eb7150c283b530b97b21f868c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.4 MB (362425984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fabac6e9d8c84d310fd6d24ee9b91f3490357ef07cd7574cb9dc87bdde73d8e1`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 15 Jan 2021 00:05:48 GMT
ADD file:ad2b2ddca8e17229cc8d1380ecda32c4b2c04f1e2aed8f493f745c6352b34e60 in / 
# Fri, 15 Jan 2021 00:05:49 GMT
CMD ["/bin/bash"]
# Fri, 15 Jan 2021 00:43:36 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 15 Jan 2021 00:43:38 GMT
ENV LANG=C.UTF-8
# Fri, 15 Jan 2021 00:46:48 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 15 Jan 2021 00:46:49 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Jan 2021 22:48:03 GMT
ENV JAVA_VERSION=16-ea+32
# Fri, 15 Jan 2021 22:49:01 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/32/GPL/openjdk-16-ea+32_linux-aarch64_bin.tar.gz; 			downloadSha256=c4ccb6df63b7b973504ad4dec0164d308d5dce7a5e2dcc508180deda33d4e61a; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/32/GPL/openjdk-16-ea+32_linux-x64_bin.tar.gz; 			downloadSha256=c951c0f2d55bc67fecbe0913675811721d13de16f4a81bf5363b660d17c02f0b; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 15 Jan 2021 22:49:04 GMT
CMD ["jshell"]
# Sat, 16 Jan 2021 00:28:23 GMT
ARG MAVEN_VERSION=3.6.3
# Sat, 16 Jan 2021 00:28:23 GMT
ARG USER_HOME_DIR=/root
# Sat, 16 Jan 2021 00:28:24 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Sat, 16 Jan 2021 00:28:25 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Sat, 16 Jan 2021 00:29:50 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN microdnf install findutils git
# Sat, 16 Jan 2021 00:30:02 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 16 Jan 2021 00:30:03 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 16 Jan 2021 00:30:04 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 16 Jan 2021 00:30:05 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 16 Jan 2021 00:30:05 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 16 Jan 2021 00:30:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 16 Jan 2021 00:30:07 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d0eecbd2c3e7306adbf5b4a0d9bebc7d266ebe78bda044d35b0994c1cf655a54`  
		Last Modified: Wed, 06 Jan 2021 20:47:00 GMT  
		Size: 42.0 MB (41996293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8f86f1d6521cdc8416801b8dd0b15d9a5a85bfa3eb8f9afa832aa8cc652732`  
		Last Modified: Fri, 15 Jan 2021 00:55:15 GMT  
		Size: 14.1 MB (14057398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d1278f211ac54faae9306e9dda291d7e00388b5b672542d754d9a70a628173`  
		Last Modified: Fri, 15 Jan 2021 22:59:17 GMT  
		Size: 179.1 MB (179130770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae4139ac43bacf26977d131698a90a59d0b11263b4ddd739b60facbadc88407`  
		Last Modified: Sat, 16 Jan 2021 00:34:27 GMT  
		Size: 117.7 MB (117659110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d05c99f24cb8b28d442d7d30b648c64bdf4d0497119003bf0debe45d40f597`  
		Last Modified: Sat, 16 Jan 2021 00:34:13 GMT  
		Size: 9.6 MB (9581196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4719c963a9ac6136d17e6a04f0625c612961410769c7bf2845c8b1f0ab7be2e8`  
		Last Modified: Sat, 16 Jan 2021 00:34:07 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de1b562a7430f785409f7fa70ae3ccbc2ae031aecaac35e4dcbee8a68ffdfd1`  
		Last Modified: Sat, 16 Jan 2021 00:34:08 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
