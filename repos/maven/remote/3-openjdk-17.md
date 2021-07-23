## `maven:3-openjdk-17`

```console
$ docker pull maven@sha256:e462ee0c51838b73262f6d00c34ff18774452e73b7695a7ba9786613e53bfd9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-17` - linux; amd64

```console
$ docker pull maven@sha256:0cf3851bb306f80f640f70b9ac4ad7f72580d5cd0e2aceaf30133ce90ae8db2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.6 MB (419636440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73e7fecf86de7aa93f0770b145b7d1e0cdf24c9fb56096c06ec30bae26fe6a51`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 12 Jul 2021 20:20:57 GMT
ADD file:c830de449b9ecd90e02f56d99e8326701da17970fa314bd7b060fd9a7cf7ac77 in / 
# Mon, 12 Jul 2021 20:20:58 GMT
CMD ["/bin/bash"]
# Mon, 12 Jul 2021 23:33:03 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 12 Jul 2021 23:34:11 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Mon, 12 Jul 2021 23:34:11 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 12 Jul 2021 23:34:12 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jul 2021 22:21:49 GMT
ENV JAVA_VERSION=17-ea+31
# Thu, 15 Jul 2021 22:22:08 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/31/GPL/openjdk-17-ea+31_linux-x64_bin.tar.gz'; 			downloadSha256='b66b6d200604e1bfa5d5642162626601d262756a6f313d1b8532dec41c870ab0'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/31/GPL/openjdk-17-ea+31_linux-aarch64_bin.tar.gz'; 			downloadSha256='6879cd8978ad5b00cbf56ee2c1b297142ff0a6017df29a66ffa80b8aa864037f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 15 Jul 2021 22:22:09 GMT
CMD ["jshell"]
# Thu, 15 Jul 2021 23:02:58 GMT
ARG MAVEN_VERSION=3.8.1
# Thu, 15 Jul 2021 23:02:59 GMT
ARG USER_HOME_DIR=/root
# Thu, 15 Jul 2021 23:02:59 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Thu, 15 Jul 2021 23:02:59 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Thu, 15 Jul 2021 23:03:26 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN microdnf install findutils git
# Thu, 15 Jul 2021 23:03:31 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Thu, 15 Jul 2021 23:03:31 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 15 Jul 2021 23:03:31 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 15 Jul 2021 23:03:31 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 15 Jul 2021 23:03:32 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Thu, 15 Jul 2021 23:03:32 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 15 Jul 2021 23:03:32 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:c828c776e142cb23ad61c84403bb42deaa97efeda5e2b600df46f7dbd38ec681`  
		Last Modified: Mon, 12 Jul 2021 20:22:25 GMT  
		Size: 42.2 MB (42179737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8846dac42cae4499c0917b5bd5e81c0e6d6fcc5326d50972b3faed7ccdf688b8`  
		Last Modified: Mon, 12 Jul 2021 23:41:34 GMT  
		Size: 13.4 MB (13392657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f431879d4af78eb52d124806d37128625e6ab6212c9817b6cf7dcf5a8b5327d6`  
		Last Modified: Thu, 15 Jul 2021 22:30:46 GMT  
		Size: 187.1 MB (187125942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01367a9cadc031d850f9728435e98f2b9b6e8dd43e3ff0fa5b21f38a4b90c7d1`  
		Last Modified: Thu, 15 Jul 2021 23:06:54 GMT  
		Size: 167.3 MB (167325927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2705918545c1426d4cc00743ec2d04e409f0407c7eba0e4c5c9ad2c4de68c75`  
		Last Modified: Thu, 15 Jul 2021 23:06:35 GMT  
		Size: 9.6 MB (9610959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d697e93e5c20861fe5dfc296c8fe691efb7d825898ea9fd257dd7879d38339c`  
		Last Modified: Thu, 15 Jul 2021 23:06:34 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5675e9ee0a50aa3268965de5c2f63e4d670999e2ec169861461c8946abb7b33`  
		Last Modified: Thu, 15 Jul 2021 23:06:34 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-17` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:f6e850bd06653b3f7966e18b9f0e272707a97cb198077ff7404fb9389d130457
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **401.2 MB (401246187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17a29dbd45d6c2f7e24f07ab5f6bf5ce1a186eb545e7faae6267c409ffa2665d`
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
# Fri, 23 Jul 2021 04:34:49 GMT
ENV JAVA_VERSION=17-ea+31
# Fri, 23 Jul 2021 04:34:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/31/GPL/openjdk-17-ea+31_linux-x64_bin.tar.gz'; 			downloadSha256='b66b6d200604e1bfa5d5642162626601d262756a6f313d1b8532dec41c870ab0'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/31/GPL/openjdk-17-ea+31_linux-aarch64_bin.tar.gz'; 			downloadSha256='6879cd8978ad5b00cbf56ee2c1b297142ff0a6017df29a66ffa80b8aa864037f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jul 2021 04:34:59 GMT
CMD ["jshell"]
# Fri, 23 Jul 2021 06:51:53 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 23 Jul 2021 06:51:53 GMT
ARG USER_HOME_DIR=/root
# Fri, 23 Jul 2021 06:51:53 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 23 Jul 2021 06:51:53 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 23 Jul 2021 06:52:16 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN microdnf install findutils git
# Fri, 23 Jul 2021 06:52:23 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 23 Jul 2021 06:52:23 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 23 Jul 2021 06:52:23 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 23 Jul 2021 06:52:24 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 23 Jul 2021 06:52:24 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 23 Jul 2021 06:52:24 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 23 Jul 2021 06:52:24 GMT
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
	-	`sha256:e9ebdeccb237bdbc57b85eb83d1fab19b1a89c6ec6126b7a1d3b4f9fd5503f35`  
		Last Modified: Fri, 23 Jul 2021 04:47:11 GMT  
		Size: 185.9 MB (185930129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e602cacff03a128b549806226d9730e35cea1626f13b26cf59d3511d738c33`  
		Last Modified: Fri, 23 Jul 2021 06:57:54 GMT  
		Size: 149.5 MB (149492204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b26ef41ad89fb43488fb8be3e70238563fae6a796a290f2f2499a0c69af128`  
		Last Modified: Fri, 23 Jul 2021 06:57:39 GMT  
		Size: 9.6 MB (9610968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8804f2f3f37a4734cc32b3585cbbdb8e952361716c057e43f7eba5d6ea3f569`  
		Last Modified: Fri, 23 Jul 2021 06:57:38 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8b75901549d9e567dfb09d2e2f574108cf8d7046d2150bba2b44049e3af8f0`  
		Last Modified: Fri, 23 Jul 2021 06:57:38 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
