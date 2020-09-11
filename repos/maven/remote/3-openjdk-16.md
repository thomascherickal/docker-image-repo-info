## `maven:3-openjdk-16`

```console
$ docker pull maven@sha256:8307dae9bfbd146ebbc821b8a692596c8fa1445871ba72be989911b71a243647
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-openjdk-16` - linux; amd64

```console
$ docker pull maven@sha256:20a299dd392633a7720a246f820fafbc6c2dd8223572a0eec444ae515c618522
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.8 MB (351783215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648b7a7b349428938e5af56b65aa999f0c43d4aaf16c47ff4a2186d4c8154797`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Fri, 11 Sep 2020 09:49:59 GMT
ADD file:50f1210cda2b0463fc72e0e56a1636cc26b6685c08c7e2cabf7fc2329b04537b in / 
# Fri, 11 Sep 2020 09:49:59 GMT
CMD ["/bin/bash"]
# Fri, 11 Sep 2020 10:23:52 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Sep 2020 10:23:52 GMT
ENV LANG=C.UTF-8
# Fri, 11 Sep 2020 10:23:52 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 11 Sep 2020 10:23:52 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Sep 2020 10:23:53 GMT
ENV JAVA_VERSION=16-ea+14
# Fri, 11 Sep 2020 10:24:29 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/14/GPL/openjdk-16-ea+14_linux-aarch64_bin.tar.gz; 			downloadSha256=4924fb671a224f19c55fb3e74e3ed7bea9b32e76545671803204997e8b7b24bf; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/14/GPL/openjdk-16-ea+14_linux-x64_bin.tar.gz; 			downloadSha256=c5006de0056bf35a4fafcf28c24f5a9a96078c704b074cdb58b00dec463b1488; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Sep 2020 10:24:29 GMT
CMD ["jshell"]
# Fri, 11 Sep 2020 11:03:33 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 11 Sep 2020 11:03:33 GMT
ARG USER_HOME_DIR=/root
# Fri, 11 Sep 2020 11:03:33 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 11 Sep 2020 11:03:34 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 11 Sep 2020 11:03:46 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN microdnf install findutils
# Fri, 11 Sep 2020 11:03:49 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 11 Sep 2020 11:03:50 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 11 Sep 2020 11:03:50 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 11 Sep 2020 11:03:50 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 11 Sep 2020 11:03:50 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 11 Sep 2020 11:03:50 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 11 Sep 2020 11:03:51 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:4374a5c9a09aec3eb7169ecd4f7ff91fedce7aeb23b479e5f83af47ec91c5d7c`  
		Last Modified: Fri, 11 Sep 2020 09:51:53 GMT  
		Size: 53.2 MB (53194134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628f382586998761d4d6eaf3d2f5d56829c3099ff15ff17f86c2767c85530a14`  
		Last Modified: Fri, 11 Sep 2020 10:28:24 GMT  
		Size: 13.4 MB (13409452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c223ee096d8faa396fa12df2adfa75fec3370a9f2eadfbd92c2b0d182f53442`  
		Last Modified: Fri, 11 Sep 2020 10:28:39 GMT  
		Size: 196.6 MB (196637704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeca1d82da431bddd321e374ec5b8f6b509e394cdc390e077a7204862f62323b`  
		Last Modified: Fri, 11 Sep 2020 11:05:47 GMT  
		Size: 79.0 MB (78959503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1998c29ac853db6da3ddeeac0bed32403aff087d2eef3130564ca4f2a3369a69`  
		Last Modified: Fri, 11 Sep 2020 11:05:42 GMT  
		Size: 9.6 MB (9581210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4fae5b172c9e47252749223beb56118e204401c7865fab1ee2cd1601e202aa`  
		Last Modified: Fri, 11 Sep 2020 11:05:42 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc49c40b872bf29734e2dcf431f71563786310f43eae1bac949c33650a3ca31a`  
		Last Modified: Fri, 11 Sep 2020 11:05:42 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-openjdk-16` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:1f38eaae2e6d49f4c5322ebeccd22b233ac96e3460c6930c75de505337e30a84
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.7 MB (305651920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:764ce029e585929aeeab58c2c67109c3c3a3c3592bfe0eaf0fea038261384e8b`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 31 May 2019 21:40:52 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Fri, 11 Sep 2020 06:39:42 GMT
ADD file:c8745918ce90d90daefed5ea00db8b400158109f53a85988975f96ce7084c609 in / 
# Fri, 11 Sep 2020 06:39:46 GMT
CMD ["/bin/bash"]
# Fri, 11 Sep 2020 07:09:36 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Sep 2020 07:09:38 GMT
ENV LANG=C.UTF-8
# Fri, 11 Sep 2020 07:09:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 11 Sep 2020 07:09:39 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Sep 2020 07:09:40 GMT
ENV JAVA_VERSION=16-ea+14
# Fri, 11 Sep 2020 07:10:14 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/14/GPL/openjdk-16-ea+14_linux-aarch64_bin.tar.gz; 			downloadSha256=4924fb671a224f19c55fb3e74e3ed7bea9b32e76545671803204997e8b7b24bf; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/14/GPL/openjdk-16-ea+14_linux-x64_bin.tar.gz; 			downloadSha256=c5006de0056bf35a4fafcf28c24f5a9a96078c704b074cdb58b00dec463b1488; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Sep 2020 07:10:15 GMT
CMD ["jshell"]
# Fri, 11 Sep 2020 07:36:29 GMT
ARG MAVEN_VERSION=3.6.3
# Fri, 11 Sep 2020 07:36:29 GMT
ARG USER_HOME_DIR=/root
# Fri, 11 Sep 2020 07:36:30 GMT
ARG SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0
# Fri, 11 Sep 2020 07:36:31 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries
# Fri, 11 Sep 2020 07:36:45 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN microdnf install findutils
# Fri, 11 Sep 2020 07:36:50 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.6.3/binaries MAVEN_VERSION=3.6.3 SHA=c35a1803a6e70a126e80b2b3ae33eed961f83ed74d18fcd16909b2d44d7dada3203f1ffe726c17ef8dcca2dcaa9fca676987befeadc9b9f759967a8cb77181c0 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 11 Sep 2020 07:36:51 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 11 Sep 2020 07:36:52 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 11 Sep 2020 07:36:53 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 11 Sep 2020 07:36:53 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 11 Sep 2020 07:36:54 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 11 Sep 2020 07:36:55 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:b0a89fc27ec40345cd34fac22c2caa5adb9d10c730a6bd900435007be8e8ac80`  
		Last Modified: Fri, 11 Sep 2020 06:41:50 GMT  
		Size: 53.3 MB (53291835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54565c8f5569913127216a9630522b7177b23429e528cdd38041680808117936`  
		Last Modified: Fri, 11 Sep 2020 07:13:47 GMT  
		Size: 14.3 MB (14311816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3137ed5f564ea8d0223838f480500eaf60d126cd66e6a85666a026ca271cae42`  
		Last Modified: Fri, 11 Sep 2020 07:14:12 GMT  
		Size: 175.2 MB (175218209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cc53b59ee1b0990e7da15ad579592d6087b2dadffef858190a71973c11a235`  
		Last Modified: Fri, 11 Sep 2020 07:38:27 GMT  
		Size: 53.2 MB (53247642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc143cb972c65979623586251876ce3e1df11905d044d5f7e5490bc1569c3c9`  
		Last Modified: Fri, 11 Sep 2020 07:38:21 GMT  
		Size: 9.6 MB (9581204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627f8a4bc59ac8f96522d2673a13a432de0e8092c8ac89f95588644ec8ac88e3`  
		Last Modified: Fri, 11 Sep 2020 07:38:20 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e38cbedc17233f5192b6aa2ec83a80087c2969e0d407997d6258e770cf9bed`  
		Last Modified: Fri, 11 Sep 2020 07:38:20 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
