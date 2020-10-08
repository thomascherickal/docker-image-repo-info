## `openjdk:15-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:345dc74c2887cf2fbe1a48951fc36a032209f5b2a0b19858bd9797bd74df21e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:15-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:ac035f8db148f5281c020faf4668466bc04e0fafe39a8a94b3f32297980d8cb7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.0 MB (260025659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772a9031541d09d43f7e9bd0d072ee21ae2add7a313a347e71a0ea7a17818066`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 21:23:41 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Thu, 08 Oct 2020 16:37:49 GMT
ADD file:b747df581cc38d6a653ccdef4b2b22a3ab465129d9b982a866cefb717a627cbb in / 
# Thu, 08 Oct 2020 16:37:50 GMT
CMD ["/bin/bash"]
# Thu, 08 Oct 2020 16:55:51 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 08 Oct 2020 16:55:51 GMT
ENV LANG=en_US.UTF-8
# Thu, 08 Oct 2020 16:56:34 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Thu, 08 Oct 2020 16:56:35 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Oct 2020 16:56:35 GMT
ENV JAVA_VERSION=15
# Thu, 08 Oct 2020 16:56:49 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-aarch64_bin.tar.gz; 			downloadSha256=01e7e07dd8a67a65b32fdcaff75ba3f21cd9cfc749287e7c9b1c6037f96a3537; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-x64_bin.tar.gz; 			downloadSha256=bb67cadee687d7b486583d03c9850342afea4593be4f436044d785fba9508fb7; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 08 Oct 2020 16:56:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6c36dbf3d26c0682385c39e59ea7c91d5d801ede8157648c145177059fca1106`  
		Last Modified: Thu, 08 Oct 2020 16:39:40 GMT  
		Size: 48.0 MB (48041338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147cd02797a98721c7ef28707dfd04e0663d2091dcc07295482fc2129157b722`  
		Last Modified: Thu, 08 Oct 2020 17:00:36 GMT  
		Size: 16.2 MB (16232412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f8f9bd9515e8a49af9b07a401d997f73c5759cf6452cc77182f4d42f903202`  
		Last Modified: Thu, 08 Oct 2020 17:01:43 GMT  
		Size: 195.8 MB (195751909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:90471f7279ee1c2a441d9a59b5c2e2e03435e4646e1e8d0e8fe942610ecad8ad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.9 MB (239892024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a301ed490f138884637adfd1d892c54fb23233b742d496b4023344bbc7ceb66e`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 20:41:36 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Thu, 08 Oct 2020 18:38:35 GMT
ADD file:ee7896b664af217b370300d68f776e8d7ae81958bc65f9bf27a4c9af308798fd in / 
# Thu, 08 Oct 2020 18:38:43 GMT
CMD ["/bin/bash"]
# Thu, 08 Oct 2020 20:21:31 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 08 Oct 2020 20:21:32 GMT
ENV LANG=en_US.UTF-8
# Thu, 08 Oct 2020 20:23:01 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Thu, 08 Oct 2020 20:23:02 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Oct 2020 20:23:03 GMT
ENV JAVA_VERSION=15
# Thu, 08 Oct 2020 20:23:50 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-aarch64_bin.tar.gz; 			downloadSha256=01e7e07dd8a67a65b32fdcaff75ba3f21cd9cfc749287e7c9b1c6037f96a3537; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-x64_bin.tar.gz; 			downloadSha256=bb67cadee687d7b486583d03c9850342afea4593be4f436044d785fba9508fb7; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 08 Oct 2020 20:23:52 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:96e8c5ccf3b6c8a786327b651db7c9e5f2230838cbfdc5dd0b97a54c7cdbc75c`  
		Last Modified: Thu, 08 Oct 2020 18:39:44 GMT  
		Size: 48.6 MB (48605945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28dee51605e9f233f5bf287b0dea133ab80a19e84b88d3b72fb93d3cbe422e5`  
		Last Modified: Thu, 08 Oct 2020 20:25:47 GMT  
		Size: 16.4 MB (16429256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8505ddefc9b22ab468d05fc319e22a4cc83af4adc9084bb90896f368f16cb10f`  
		Last Modified: Thu, 08 Oct 2020 20:26:56 GMT  
		Size: 174.9 MB (174856823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
