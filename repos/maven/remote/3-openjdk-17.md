## `maven:3-openjdk-17`

```console
$ docker pull maven@sha256:485ca136be91d61c9438a83187398853a5d2dc20182ce5bc6021c389b6eb2c13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-17` - linux; amd64

```console
$ docker pull maven@sha256:4d6916cfee8e188348c579cf4765a9d50c9cb0037da430682bc2bf76c07ed2d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.4 MB (397416995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fed7c671c8815d5c9e57d3a0eafad1ce3e165afabff14aa2c8c8e388c17f4c7f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Sat, 17 Apr 2021 01:21:29 GMT
ADD file:9c532b9932419aab70115bea018132ac9096e9eebb25f230bda99cb66245fab2 in / 
# Sat, 17 Apr 2021 01:21:29 GMT
CMD ["/bin/bash"]
# Sat, 17 Apr 2021 01:38:22 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 17 Apr 2021 01:38:22 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Sat, 17 Apr 2021 01:38:22 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 17 Apr 2021 01:38:22 GMT
ENV LANG=C.UTF-8
# Sat, 01 May 2021 03:39:04 GMT
ENV JAVA_VERSION=17-ea+20
# Sat, 01 May 2021 03:39:15 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='2de5c546c3e38f36676c7e22dd040e5b540fc258f72194e7ae17af3f2bf7f0b5'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='9e376a3f2c9a3dc5394fc2f3da480f72b9103c3b71d39d041dc6b08bb65e5724'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 01 May 2021 03:39:17 GMT
CMD ["jshell"]
# Sat, 01 May 2021 05:29:53 GMT
ARG MAVEN_VERSION=3.8.1
# Sat, 01 May 2021 05:29:53 GMT
ARG USER_HOME_DIR=/root
# Sat, 01 May 2021 05:29:53 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Sat, 01 May 2021 05:29:53 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Sat, 01 May 2021 05:30:16 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN microdnf install findutils git
# Sat, 01 May 2021 05:30:23 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 01 May 2021 05:30:23 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 01 May 2021 05:30:24 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 01 May 2021 05:30:24 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 01 May 2021 05:30:24 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 01 May 2021 05:30:24 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 01 May 2021 05:30:24 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:9509c6b41a37fbf5dbb93aedded1aff0dc6ed45ab2d334440e10a5c8d112531c`  
		Last Modified: Sat, 17 Apr 2021 01:22:39 GMT  
		Size: 42.1 MB (42063762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0005db77786a07e4e5d56adc224c9dc85320b46354f9110eb174ce7df9df04`  
		Last Modified: Sat, 17 Apr 2021 01:43:53 GMT  
		Size: 13.3 MB (13272982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5f496cc317d0c1629ec3441d92034406388aa49e7ac7f629c6a732c02c919`  
		Last Modified: Sat, 01 May 2021 03:44:27 GMT  
		Size: 186.0 MB (186001799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b79fb2e5d26c92e41491fce13c2925435b7ff669bd77b3a1bdd22d7bf47ed67`  
		Last Modified: Sat, 01 May 2021 05:33:26 GMT  
		Size: 146.5 MB (146466255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7ab253a3bf79328a292df0fe63ccf259d845249bb6f07b322aa82546a0da27`  
		Last Modified: Sat, 01 May 2021 05:33:11 GMT  
		Size: 9.6 MB (9610981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fb780c9889aeb6e543f38f37f703b873b349be8e7a8450173340e81ed4abe2`  
		Last Modified: Sat, 01 May 2021 05:33:09 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a44891e8ba8aad51c81f3957c7c314e74bb62ad2a3d8c0b272306f9b9955d38`  
		Last Modified: Sat, 01 May 2021 05:33:09 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-17` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:053cde7bcbe66a4f8683d71472ab32e0d8998a767ca8fa3a6ab01d098fca8a84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.7 MB (376658481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:153824680f6281c364341bff335ee7b615de391c16d618246d6fb57b222bd5a6`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Sat, 17 Apr 2021 00:43:47 GMT
ADD file:2afad2b68d4889be2ef517aea246957975145f8ad99a3e9e6a01baf79f67d5e2 in / 
# Sat, 17 Apr 2021 00:43:51 GMT
CMD ["/bin/bash"]
# Sat, 17 Apr 2021 01:01:42 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 17 Apr 2021 01:01:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Sat, 17 Apr 2021 01:01:44 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 17 Apr 2021 01:01:45 GMT
ENV LANG=C.UTF-8
# Sat, 01 May 2021 01:17:50 GMT
ENV JAVA_VERSION=17-ea+20
# Sat, 01 May 2021 01:18:46 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='2de5c546c3e38f36676c7e22dd040e5b540fc258f72194e7ae17af3f2bf7f0b5'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/20/GPL/openjdk-17-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='9e376a3f2c9a3dc5394fc2f3da480f72b9103c3b71d39d041dc6b08bb65e5724'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 01 May 2021 01:18:50 GMT
CMD ["jshell"]
# Sat, 01 May 2021 03:26:32 GMT
ARG MAVEN_VERSION=3.8.1
# Sat, 01 May 2021 03:26:32 GMT
ARG USER_HOME_DIR=/root
# Sat, 01 May 2021 03:26:33 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Sat, 01 May 2021 03:26:35 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Sat, 01 May 2021 03:27:59 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN microdnf install findutils git
# Sat, 01 May 2021 03:28:07 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 01 May 2021 03:28:08 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 01 May 2021 03:28:11 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 01 May 2021 03:28:12 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 01 May 2021 03:28:13 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 01 May 2021 03:28:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 01 May 2021 03:28:16 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:4b26d50a92155f32c82c580c6abd80083d4fff230a35ef647094df38f4475f9f`  
		Last Modified: Sat, 17 Apr 2021 00:45:12 GMT  
		Size: 42.0 MB (41996718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc97fa408166ea1b3901653a092a35a895b8718e00810a9bf87dd8f1d0430f3`  
		Last Modified: Sat, 17 Apr 2021 01:07:39 GMT  
		Size: 14.0 MB (14034435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5622382afc27f54718bfb4da11613ae12eee4e86b910c18045a465a61e39cb1f`  
		Last Modified: Sat, 01 May 2021 01:26:32 GMT  
		Size: 182.1 MB (182081386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5a1ec2178446234d58fc71d1d22b5645dc77b917f8e9a74143d0f760200123`  
		Last Modified: Sat, 01 May 2021 03:32:15 GMT  
		Size: 128.9 MB (128933736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cdc90a61a85011f12539b9d5d2126f7844b472535097fc7a0bba2771acb05b`  
		Last Modified: Sat, 01 May 2021 03:31:54 GMT  
		Size: 9.6 MB (9610989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c72c0510510caedce436626c4310c2f7f0a7810ffb76d99fac20914c10beb4d`  
		Last Modified: Sat, 01 May 2021 03:31:53 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a023c78c92862f6fb91ce22e7d2a237ccd75c7509ce5734e7079f2d4213689`  
		Last Modified: Sat, 01 May 2021 03:31:53 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
