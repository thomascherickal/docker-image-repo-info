## `openjdk:15-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:f21634c92e8e8c3e1715b8b206daebebc0298a9973f6b63fb095d42163e5245a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:15-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:4026186908886bb122b9e760f72b95ed240eb5cf2d48487b3c86a3c555123650
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.4 MB (263449756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95b80f783bd241b9896f1a66c312d670eb8a6b5cb71f6d45976438b1fa476589`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 21:22:07 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Fri, 30 Oct 2020 02:05:51 GMT
ADD file:ca74b6a4572ba9ecd7ceca8360a2d15560bf779277672ae9a37e25c53f8d1226 in / 
# Fri, 30 Oct 2020 02:05:51 GMT
CMD ["/bin/bash"]
# Fri, 30 Oct 2020 04:37:30 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 30 Oct 2020 04:37:30 GMT
ENV LANG=C.UTF-8
# Fri, 30 Oct 2020 04:39:24 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 30 Oct 2020 04:39:24 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Oct 2020 04:39:25 GMT
ENV JAVA_VERSION=15.0.1
# Fri, 30 Oct 2020 04:39:40 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.1/51f4f36ad4ef43e39d0dfdbaf6549e32/9/GPL/openjdk-15.0.1_linux-aarch64_bin.tar.gz; 			downloadSha256=6a62b7ec065280bad978a3322733a089153dec5ebf5ba81fd2fa361382dbc7b0; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.1/51f4f36ad4ef43e39d0dfdbaf6549e32/9/GPL/openjdk-15.0.1_linux-x64_bin.tar.gz; 			downloadSha256=83ec3a7b1649a6b31e021cde1e58ab447b07fb8173489f27f427e731c89ed84a; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 30 Oct 2020 04:39:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9f8aeb516aa1b01143452930dec1cadef36b4298bcdb43224755b12ab4bc9289`  
		Last Modified: Fri, 30 Oct 2020 02:07:57 GMT  
		Size: 54.2 MB (54163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6199265ff0195874d7975d360d91e2ed48bc621c12633d52a4fe5207953ff202`  
		Last Modified: Fri, 30 Oct 2020 04:42:34 GMT  
		Size: 13.5 MB (13508533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5614451d1903a5b3955552f1f4a3d94f61477ccc34d7e1521a4029c7c7b15185`  
		Last Modified: Fri, 30 Oct 2020 04:44:10 GMT  
		Size: 195.8 MB (195778204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:ae6f1e5572dcb82df51e6857cab41787181e51dff217bde6dc63719ded56ca73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243521740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c768a0384f88bbbd67bebafbbba7f40edb67fa815ab661b71eb28f2181abc219`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 20:40:54 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Fri, 30 Oct 2020 03:44:45 GMT
ADD file:9cec0313dda06011e5a2f413448db8dc2a3f2e6305dbfd3afa2f78c9e571c080 in / 
# Fri, 30 Oct 2020 03:44:49 GMT
CMD ["/bin/bash"]
# Fri, 30 Oct 2020 04:03:41 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 30 Oct 2020 04:03:42 GMT
ENV LANG=C.UTF-8
# Fri, 30 Oct 2020 04:07:39 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 30 Oct 2020 04:07:39 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 30 Oct 2020 04:07:40 GMT
ENV JAVA_VERSION=15.0.1
# Fri, 30 Oct 2020 04:08:20 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.1/51f4f36ad4ef43e39d0dfdbaf6549e32/9/GPL/openjdk-15.0.1_linux-aarch64_bin.tar.gz; 			downloadSha256=6a62b7ec065280bad978a3322733a089153dec5ebf5ba81fd2fa361382dbc7b0; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.1/51f4f36ad4ef43e39d0dfdbaf6549e32/9/GPL/openjdk-15.0.1_linux-x64_bin.tar.gz; 			downloadSha256=83ec3a7b1649a6b31e021cde1e58ab447b07fb8173489f27f427e731c89ed84a; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 30 Oct 2020 04:08:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e3e30b00fc3497706dcd32508109092c83b0a5b47bd1dbd485dc8a0da352da68`  
		Last Modified: Fri, 30 Oct 2020 03:46:38 GMT  
		Size: 54.3 MB (54268366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2870a34311e6e2480637a34f3904b567d224baff73277563033ebcee672d93`  
		Last Modified: Fri, 30 Oct 2020 04:11:09 GMT  
		Size: 14.4 MB (14365455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb7875e0f30d614362575a6486505e1aa3bc619b289716bcb19255f9574d523`  
		Last Modified: Fri, 30 Oct 2020 04:12:16 GMT  
		Size: 174.9 MB (174887919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
