## `maven:3-openjdk-16`

```console
$ docker pull maven@sha256:3dce76f84ec6eaaf47876562d23ed162afbcf1793d2e7fbb2c8ef38baf28e48d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-16` - linux; amd64

```console
$ docker pull maven@sha256:d99045d9b4f63b8cf8bedf60d0e3011312135a5a3c13518bfeb57b0d565f00e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.3 MB (353305808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0f1a2a47f1bfeb04d5ba15b942a2890483360c7552dc5e3a368a801eaf0c9b3`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 15 Sep 2020 21:22:07 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Tue, 15 Sep 2020 21:22:13 GMT
ADD file:8011e31575cbf4b8ebb243821b300ba24330e02cab925024aa98f4ce27997846 in / 
# Tue, 15 Sep 2020 21:22:13 GMT
CMD ["/bin/bash"]
# Tue, 15 Sep 2020 21:41:02 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 15 Sep 2020 21:41:02 GMT
ENV LANG=C.UTF-8
# Tue, 15 Sep 2020 21:41:02 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Tue, 15 Sep 2020 21:41:02 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Oct 2020 01:59:38 GMT
ENV JAVA_VERSION=16-ea+18
# Fri, 02 Oct 2020 02:00:40 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/18/GPL/openjdk-16-ea+18_linux-aarch64_bin.tar.gz; 			downloadSha256=89d569c7a8eec74a029fbc2788348bf47ca8bb62ebb1433070b2044d0930ff92; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/18/GPL/openjdk-16-ea+18_linux-x64_bin.tar.gz; 			downloadSha256=780cd45198c4d32796b685683cca0cb0c300e4ee1607798ac1197dc36040e3b9; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 02 Oct 2020 02:00:41 GMT
CMD ["jshell"]
# Fri, 02 Oct 2020 05:34:52 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 02 Oct 2020 05:34:52 GMT
ARG USER_HOME_DIR=/root
# Fri, 02 Oct 2020 05:34:52 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 02 Oct 2020 05:34:52 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 02 Oct 2020 05:35:06 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN microdnf install findutils
# Fri, 02 Oct 2020 05:35:09 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 02 Oct 2020 05:35:09 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 02 Oct 2020 05:35:09 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 02 Oct 2020 05:35:09 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 02 Oct 2020 05:35:10 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 02 Oct 2020 05:35:10 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 02 Oct 2020 05:35:10 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:79701ada7495177c292979fd69d41eee91dc93ef0feea5ff95bb453f4ab7a1c5`  
		Last Modified: Mon, 14 Sep 2020 18:35:00 GMT  
		Size: 54.2 MB (54164063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47708145bbc56f1e73084e03c4662a6b29535708cfe5d51510cdae37bc363ba3`  
		Last Modified: Tue, 15 Sep 2020 21:47:10 GMT  
		Size: 13.5 MB (13491818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0008c388567c120679a244c559b44297ef05aad04b18d4aaada12f7fb3be4a`  
		Last Modified: Fri, 02 Oct 2020 02:05:02 GMT  
		Size: 196.5 MB (196497912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34657210508fb2b90da6ab7152e1ed8ec0d2f3d80c9ef9c100a830c6d79ac780`  
		Last Modified: Fri, 02 Oct 2020 05:36:46 GMT  
		Size: 79.6 MB (79569585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232a22adf39f57526a90ca7e60702eafab270f7c8c62b6ebaf935823b61266fb`  
		Last Modified: Fri, 02 Oct 2020 05:36:42 GMT  
		Size: 9.6 MB (9581209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17873b54f6c6af0b13453fde0f99174200a57ae8f58db15b5c75b83a4dd90937`  
		Last Modified: Fri, 02 Oct 2020 05:36:41 GMT  
		Size: 861.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d0d595f72980c02f201e48e11f349725c0c4d4a901438da161872da6c41dc4`  
		Last Modified: Fri, 02 Oct 2020 05:36:41 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-16` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:9e9be1ad1d0c3d7ede9fdce5d23173488db898eea15d07f586e7b5b6bd2b8bcd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.6 MB (308599786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20fee57b6040d44692270e59090a47927c84c1fdc51d23cf31bdcb635147dff6`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 15 Sep 2020 20:40:54 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Tue, 15 Sep 2020 20:41:01 GMT
ADD file:b3bd5c2ec8ff0efe8a0b1384563b42f02d6bcf7531132d9ec4748ecfe264d476 in / 
# Tue, 15 Sep 2020 20:41:02 GMT
CMD ["/bin/bash"]
# Tue, 15 Sep 2020 20:58:24 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 15 Sep 2020 20:58:31 GMT
ENV LANG=C.UTF-8
# Tue, 15 Sep 2020 20:58:37 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Tue, 15 Sep 2020 20:58:39 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Oct 2020 23:15:21 GMT
ENV JAVA_VERSION=16-ea+18
# Thu, 01 Oct 2020 23:16:42 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/18/GPL/openjdk-16-ea+18_linux-aarch64_bin.tar.gz; 			downloadSha256=89d569c7a8eec74a029fbc2788348bf47ca8bb62ebb1433070b2044d0930ff92; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/18/GPL/openjdk-16-ea+18_linux-x64_bin.tar.gz; 			downloadSha256=780cd45198c4d32796b685683cca0cb0c300e4ee1607798ac1197dc36040e3b9; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 01 Oct 2020 23:16:44 GMT
CMD ["jshell"]
# Fri, 02 Oct 2020 04:11:35 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 02 Oct 2020 04:11:36 GMT
ARG USER_HOME_DIR=/root
# Fri, 02 Oct 2020 04:11:37 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 02 Oct 2020 04:11:41 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 02 Oct 2020 04:12:19 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN microdnf install findutils
# Fri, 02 Oct 2020 04:12:27 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 02 Oct 2020 04:12:28 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 02 Oct 2020 04:12:28 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 02 Oct 2020 04:12:29 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 02 Oct 2020 04:12:30 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 02 Oct 2020 04:12:30 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 02 Oct 2020 04:12:31 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a805b9845b615e5963d09def3e5e9919b39e76b5122c2abecc98d4a4bb358394`  
		Last Modified: Mon, 14 Sep 2020 17:43:27 GMT  
		Size: 54.3 MB (54266593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f893975677f1e890e793bb79d6684177489551bc055499096c3c153bc305e940`  
		Last Modified: Tue, 15 Sep 2020 21:04:39 GMT  
		Size: 14.4 MB (14366569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69b874edfa9d6372d865a8048153529df92f585a468b91aba14fa1b60110ea4`  
		Last Modified: Thu, 01 Oct 2020 23:23:51 GMT  
		Size: 175.2 MB (175224790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b182364db0842f0c256604645b7056321224b726596a993ba32ae22f452de94`  
		Last Modified: Fri, 02 Oct 2020 04:15:41 GMT  
		Size: 55.2 MB (55159412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109c1897a452854893b8cd03b324e247469e5fcfa70afb6e48a2abe23edf42ea`  
		Last Modified: Fri, 02 Oct 2020 04:15:37 GMT  
		Size: 9.6 MB (9581203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb89240171c2ef921e1817be8cb3158fb7614f7cbf40c797ea2b010ffcc83cdc`  
		Last Modified: Fri, 02 Oct 2020 04:15:34 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6c4265ff659a2fb79998b43ec193c7d43a6c12185b545789750d3d4fe3134d`  
		Last Modified: Fri, 02 Oct 2020 04:15:35 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
