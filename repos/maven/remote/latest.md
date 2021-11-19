## `maven:latest`

```console
$ docker pull maven@sha256:8a66581a077762c8752a9f64f73cdd8c59e9c4446eb810417119e0436b075931
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:latest` - linux; amd64

```console
$ docker pull maven@sha256:9c31c89f38703a5ebe23741eb1760d88f9224b9fb5cf5e596df5549237cefd6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **421.8 MB (421842963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9ddcb8259eacded5b9d02f6a4a0966095d1871d5565cfdd0e1ff7501127ff2`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 19 Nov 2021 03:08:35 GMT
ADD file:d27591ceabbe39902d88042ebe31aecc38844787fafa004cdeb0080da29c1623 in / 
# Fri, 19 Nov 2021 03:08:35 GMT
CMD ["/bin/bash"]
# Fri, 19 Nov 2021 03:25:16 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 19 Nov 2021 03:25:55 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 19 Nov 2021 03:25:55 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Nov 2021 03:25:55 GMT
ENV LANG=C.UTF-8
# Fri, 19 Nov 2021 03:25:56 GMT
ENV JAVA_VERSION=17.0.1
# Fri, 19 Nov 2021 03:26:07 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='1c0a73cbb863aad579b967316bf17673b8f98a9bb938602a140ba2e5c38f880a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='86653d48787e5a1c029df10da7808194fe8bd931ddd72ff3d42850bf1afb317e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 19 Nov 2021 03:26:07 GMT
CMD ["jshell"]
# Fri, 19 Nov 2021 03:59:00 GMT
ARG MAVEN_VERSION=3.8.3
# Fri, 19 Nov 2021 03:59:01 GMT
ARG USER_HOME_DIR=/root
# Fri, 19 Nov 2021 03:59:01 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Fri, 19 Nov 2021 03:59:01 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Fri, 19 Nov 2021 03:59:29 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN microdnf install findutils git
# Fri, 19 Nov 2021 03:59:38 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 19 Nov 2021 03:59:38 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 19 Nov 2021 03:59:38 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 19 Nov 2021 03:59:39 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 19 Nov 2021 03:59:39 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 19 Nov 2021 03:59:39 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 19 Nov 2021 03:59:39 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:28587b6e64756a60a354301d011190fb69ea1eed25d7a5180811dab252e16a21`  
		Last Modified: Fri, 19 Nov 2021 03:09:27 GMT  
		Size: 42.1 MB (42097812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1655352c888337fbd3af21c25aa26d4561a0b9b6035a8b22c9ee0c8ae9a3784`  
		Last Modified: Fri, 19 Nov 2021 03:31:40 GMT  
		Size: 13.5 MB (13511818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9646f00e96d7c315cc4e7a61c091ac85314d738b5c12f5a05566e9af31f65f`  
		Last Modified: Fri, 19 Nov 2021 03:33:03 GMT  
		Size: 187.2 MB (187170401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd514e60c464ca3fba9d034d65f6114732af20e956435c4c5e7099d54aeb843`  
		Last Modified: Fri, 19 Nov 2021 04:01:45 GMT  
		Size: 170.0 MB (169956096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab2a7ea62caace9e51244949533ba71069cb400c95f2580664af20c5b7187aa`  
		Last Modified: Fri, 19 Nov 2021 04:01:31 GMT  
		Size: 9.1 MB (9105621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72072d9f9d3e6d0ec96e57732c664dd43ee00e29f9718bbde64dbdd50977ba5`  
		Last Modified: Fri, 19 Nov 2021 04:01:30 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eca236510fe4bc273bbbcfa05d5d9a012fb4a28271159741dd14e922cf322f1`  
		Last Modified: Fri, 19 Nov 2021 04:01:30 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:latest` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:907d22fe8db8a6410a6986bbd7e99f309cdb53c638f46033c359a393c7219d24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **405.4 MB (405373887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2164384bb329c490fa7f5a672d555ac44144ed3ad7dbf16fceacd1a77025944`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 19 Nov 2021 02:35:27 GMT
ADD file:31ec2bba02fab51f683553c78815a422089e6227bd4a65d33f35bc15588da3f7 in / 
# Fri, 19 Nov 2021 02:35:27 GMT
CMD ["/bin/bash"]
# Fri, 19 Nov 2021 02:52:30 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 19 Nov 2021 02:53:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Fri, 19 Nov 2021 02:53:34 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Nov 2021 02:53:35 GMT
ENV LANG=C.UTF-8
# Fri, 19 Nov 2021 02:53:36 GMT
ENV JAVA_VERSION=17.0.1
# Fri, 19 Nov 2021 02:53:48 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='1c0a73cbb863aad579b967316bf17673b8f98a9bb938602a140ba2e5c38f880a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='86653d48787e5a1c029df10da7808194fe8bd931ddd72ff3d42850bf1afb317e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 19 Nov 2021 02:53:49 GMT
CMD ["jshell"]
# Fri, 19 Nov 2021 03:26:33 GMT
ARG MAVEN_VERSION=3.8.3
# Fri, 19 Nov 2021 03:26:34 GMT
ARG USER_HOME_DIR=/root
# Fri, 19 Nov 2021 03:26:35 GMT
ARG SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa
# Fri, 19 Nov 2021 03:26:36 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries
# Fri, 19 Nov 2021 03:27:01 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN microdnf install findutils git
# Fri, 19 Nov 2021 03:27:07 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.3/binaries MAVEN_VERSION=3.8.3 SHA=1c12a5df43421795054874fd54bb8b37d242949133b5bf6052a063a13a93f13a20e6e9dae2b3d85b9c7034ec977bbc2b6e7f66832182b9c863711d78bfe60faa USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 19 Nov 2021 03:27:07 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 19 Nov 2021 03:27:08 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 19 Nov 2021 03:27:10 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 19 Nov 2021 03:27:11 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 19 Nov 2021 03:27:11 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 19 Nov 2021 03:27:12 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:c621c1ca8ceb7b3c3055633f5e537023039566ffcde238e41463f74eb6396051`  
		Last Modified: Fri, 19 Nov 2021 02:36:28 GMT  
		Size: 42.0 MB (42011387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d87024ee2f6936bf9ad81953e5ec643cddc67e7055ec11cf737242c60e2c9b`  
		Last Modified: Fri, 19 Nov 2021 03:04:14 GMT  
		Size: 14.3 MB (14300939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a3cf2319a2c8e288d9e26d8257b0b89dc0c8402f53ff80f3bf1a31553d891c`  
		Last Modified: Fri, 19 Nov 2021 03:05:51 GMT  
		Size: 186.0 MB (185977108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7492f0e5e52e748300dcefaa009d98916e3423dd4235c3cf89334b79cbf162c`  
		Last Modified: Fri, 19 Nov 2021 03:30:36 GMT  
		Size: 154.0 MB (153977675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ac3ecd9fc403231e84a5edbeafbf6ca5ba03d1a721d1cf345ed610032338d6`  
		Last Modified: Fri, 19 Nov 2021 03:30:21 GMT  
		Size: 9.1 MB (9105563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543d814ccf214bb3e1e8eb2a6f9aa5b4e1fd8ab107c54dbadbc0d03edcbf21ef`  
		Last Modified: Fri, 19 Nov 2021 03:30:20 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e2c4244efdeaeed381d8df114e615a2883915480adb1fbf414b86fb6148be0`  
		Last Modified: Fri, 19 Nov 2021 03:30:20 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
