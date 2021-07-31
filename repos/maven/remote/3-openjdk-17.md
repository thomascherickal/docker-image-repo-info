## `maven:3-openjdk-17`

```console
$ docker pull maven@sha256:f372fa37c1e7a9aa1c6cba3c530204db497d7c2468d502b4c67363df8b73f54a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-17` - linux; amd64

```console
$ docker pull maven@sha256:b7e2f33a77cbd7430175c85bb2c8c724d961fdea09fb4f0b2207cb247c9c8f43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **421.7 MB (421696274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f9969a5c2823e3fbc3d9d1e1478ab67243b9caf2c36ec66c5241529a3c9bba`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 23 Jul 2021 01:13:10 GMT
ADD file:c047ac1784a3670f52d12ad67cf238654237149dc2c9d7b921cd005c7ec42105 in / 
# Fri, 23 Jul 2021 01:13:11 GMT
CMD ["/bin/bash"]
# Fri, 23 Jul 2021 06:40:31 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 23 Jul 2021 06:41:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 23 Jul 2021 06:41:12 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:41:13 GMT
ENV LANG=C.UTF-8
# Fri, 30 Jul 2021 18:50:11 GMT
ENV JAVA_VERSION=17-ea+33
# Fri, 30 Jul 2021 18:50:22 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/33/GPL/openjdk-17-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='d89e04f161553560c454bf263924dc49c5c2529698ef8131baff632355baea18'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/33/GPL/openjdk-17-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='d361654c87bae6712f36d7f0d27914c63fbe31f10a9a0d5316072b3c69ed2263'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 30 Jul 2021 18:50:23 GMT
CMD ["jshell"]
# Fri, 30 Jul 2021 20:12:59 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 30 Jul 2021 20:13:00 GMT
ARG USER_HOME_DIR=/root
# Fri, 30 Jul 2021 20:13:00 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 30 Jul 2021 20:13:00 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 30 Jul 2021 20:13:39 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN microdnf install findutils git
# Fri, 30 Jul 2021 20:13:43 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 30 Jul 2021 20:13:43 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 30 Jul 2021 20:13:43 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 30 Jul 2021 20:13:43 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 30 Jul 2021 20:13:43 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 30 Jul 2021 20:13:44 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 30 Jul 2021 20:13:44 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:1da50e1664e1b58d93182fe5af093c642668ec93f67fcd8215b9c1979930b84d`  
		Last Modified: Fri, 23 Jul 2021 01:14:27 GMT  
		Size: 42.2 MB (42178827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c8e5a84542212d0126ce88facd146befb1c731fb4faafb50a7b96ad0568cd9`  
		Last Modified: Fri, 23 Jul 2021 06:49:18 GMT  
		Size: 13.4 MB (13390485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b485b3d06b17376a65c960bbfb335d1c6ebb1ecb5a289ef54682f392a2985e1c`  
		Last Modified: Fri, 30 Jul 2021 18:59:05 GMT  
		Size: 187.1 MB (187140200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92289c55b3b4cd3da2ee68c50d9f00e55bd37d69e550e1818d7a7e1ab033f72`  
		Last Modified: Fri, 30 Jul 2021 20:16:54 GMT  
		Size: 169.4 MB (169374588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479f32ec5f45f9f7705eb2e69f3405c67292548689fc0b852075dd3979a3b1e1`  
		Last Modified: Fri, 30 Jul 2021 20:16:42 GMT  
		Size: 9.6 MB (9610958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82c037d70ecb16ecb0381eef960e75119fce0eef660a22e5a72571293423da9`  
		Last Modified: Fri, 30 Jul 2021 20:16:40 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9eb44b3fb9fab97d2352cb0d73cb31f4b3a345ff53b685415a4320d592e09`  
		Last Modified: Fri, 30 Jul 2021 20:16:40 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-17` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:de175948d111f810139e237bd5fe0fc69d55ba5dcff2e12902d0391db9ee9ed8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **401.4 MB (401354854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f5d541fb5e23cdeb13329e74461172d8a31e3c323100203929f161545887bef`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 23 Jul 2021 00:50:01 GMT
ADD file:2b2b9653730f3bb9d3a6327d4b9a6b425279decd90b84755c033b95536ebe027 in / 
# Fri, 23 Jul 2021 00:50:02 GMT
CMD ["/bin/bash"]
# Fri, 23 Jul 2021 04:34:01 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 23 Jul 2021 04:34:49 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 23 Jul 2021 04:34:49 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 04:34:49 GMT
ENV LANG=C.UTF-8
# Sat, 31 Jul 2021 03:59:39 GMT
ENV JAVA_VERSION=17-ea+33
# Sat, 31 Jul 2021 04:00:03 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/33/GPL/openjdk-17-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='d89e04f161553560c454bf263924dc49c5c2529698ef8131baff632355baea18'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/33/GPL/openjdk-17-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='d361654c87bae6712f36d7f0d27914c63fbe31f10a9a0d5316072b3c69ed2263'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 31 Jul 2021 04:00:04 GMT
CMD ["jshell"]
# Sat, 31 Jul 2021 06:20:35 GMT
ARG MAVEN_VERSION=3.8.1
# Sat, 31 Jul 2021 06:20:35 GMT
ARG USER_HOME_DIR=/root
# Sat, 31 Jul 2021 06:20:35 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Sat, 31 Jul 2021 06:20:35 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Sat, 31 Jul 2021 06:20:58 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN microdnf install findutils git
# Sat, 31 Jul 2021 06:21:05 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 31 Jul 2021 06:21:05 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 31 Jul 2021 06:21:05 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 31 Jul 2021 06:21:06 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 31 Jul 2021 06:21:06 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 31 Jul 2021 06:21:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 31 Jul 2021 06:21:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a21bf021f71862240d392ffdd7f376294fa46f2729f1771f269c1a888d0aab25`  
		Last Modified: Fri, 23 Jul 2021 00:51:19 GMT  
		Size: 42.0 MB (42040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20d17a0583d5448fece8a45dc16fcd83266885f5eabbeaa44c9bcc8738ed0fa`  
		Last Modified: Fri, 23 Jul 2021 04:45:32 GMT  
		Size: 14.2 MB (14170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd2ec7b9a5f76ce87e756852ef047c8330c8c5e5055a76cf979622c398cb286`  
		Last Modified: Sat, 31 Jul 2021 04:14:38 GMT  
		Size: 186.0 MB (185956664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1164d0ef45cddc8f3054daf9d5cd4f5d02210bc5dc217de9d9f729521699ecee`  
		Last Modified: Sat, 31 Jul 2021 06:26:08 GMT  
		Size: 149.6 MB (149574320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52c598e41184a18e02547081311d703eaf99c75cbf754a6e8b49e377aab3040`  
		Last Modified: Sat, 31 Jul 2021 06:25:54 GMT  
		Size: 9.6 MB (9610982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d87e9e086266b56a79c85207c034840b3ae243f7918f1555a0bc4a75e1cf20d`  
		Last Modified: Sat, 31 Jul 2021 06:25:53 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b0e9ebc4cad09117154fd7e6584dac41e26e2f00f682d9e218194ddd220c73`  
		Last Modified: Sat, 31 Jul 2021 06:25:53 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
