## `openjdk:16-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:3120c54cf5d92ff7ead1eaed79580cc892ddffc67902a1df1228811b4db501b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:aed015aa2feb6d043252a73df5df27c0025052c804bc703a9b69089344b5a316
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (260999962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e83b0e50a4a2daad701a0063a4c6b9d0696df902858467c0f3dec636cf4bc3a1`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 21:23:41 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Tue, 15 Sep 2020 21:23:46 GMT
ADD file:0846801b1ef59a7513feb7e2704d8b0c5618da23e28ecff72f64ac14799ee0c1 in / 
# Tue, 15 Sep 2020 21:23:46 GMT
CMD ["/bin/bash"]
# Tue, 15 Sep 2020 21:42:25 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 15 Sep 2020 21:42:25 GMT
ENV LANG=en_US.UTF-8
# Tue, 15 Sep 2020 21:42:26 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Tue, 15 Sep 2020 21:42:26 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 25 Sep 2020 22:04:10 GMT
ENV JAVA_VERSION=16-ea+17
# Fri, 25 Sep 2020 22:04:30 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/17/GPL/openjdk-16-ea+17_linux-aarch64_bin.tar.gz; 			downloadSha256=e7005f023a943945defa57440bc7207cfb5f97b7ce4a0f054542948631c53cb6; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/17/GPL/openjdk-16-ea+17_linux-x64_bin.tar.gz; 			downloadSha256=b7244f2059e486aabb071dcf1be5185d86a1a723cc213d6b44551a4973d5e54f; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 25 Sep 2020 22:04:31 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bce8f778fef067eed3d092243c838d674cb1ef39441d85d0ca84382084a69093`  
		Last Modified: Fri, 17 Jul 2020 02:37:13 GMT  
		Size: 48.0 MB (48014772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a21ecfa328a07e4933d7514beae1d65556b84f84efcf20e57a8acecdb757a8d`  
		Last Modified: Tue, 15 Sep 2020 21:47:50 GMT  
		Size: 16.2 MB (16187300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54afba0898bf46e1d6ecf84d2f6974da164eeab597c51fa72d52e4e59fb09ee4`  
		Last Modified: Fri, 25 Sep 2020 22:10:21 GMT  
		Size: 196.8 MB (196797890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:3502b6a5ff4abc59aee11dd8cb5ed8a2f3c73d7df497c2cc708583d1a1d51d4b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240300120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2578db35abf7f56c375cb07551e537780750f582fbd26411499dba4b95d5c0c7`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 20:41:36 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Tue, 15 Sep 2020 20:41:43 GMT
ADD file:f07cad218c7e24e1cbce662268da25d9318627f636feebb0f669155354c7f365 in / 
# Tue, 15 Sep 2020 20:41:44 GMT
CMD ["/bin/bash"]
# Tue, 15 Sep 2020 21:00:40 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 15 Sep 2020 21:00:49 GMT
ENV LANG=en_US.UTF-8
# Tue, 15 Sep 2020 21:00:52 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Tue, 15 Sep 2020 21:00:53 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Oct 2020 23:17:11 GMT
ENV JAVA_VERSION=16-ea+18
# Thu, 01 Oct 2020 23:17:59 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/18/GPL/openjdk-16-ea+18_linux-aarch64_bin.tar.gz; 			downloadSha256=89d569c7a8eec74a029fbc2788348bf47ca8bb62ebb1433070b2044d0930ff92; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/18/GPL/openjdk-16-ea+18_linux-x64_bin.tar.gz; 			downloadSha256=780cd45198c4d32796b685683cca0cb0c300e4ee1607798ac1197dc36040e3b9; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 01 Oct 2020 23:18:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f5053e285643065e9638a069d53c6f62fd6bf1d6d4d16001d48a66ee024d7397`  
		Last Modified: Fri, 17 Jul 2020 01:45:56 GMT  
		Size: 48.6 MB (48633508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891c11a7b021d2684a0bbcbc93b7f9b3a89839303cdf3e7ff528cf95eeb11ed6`  
		Last Modified: Tue, 15 Sep 2020 21:05:28 GMT  
		Size: 16.4 MB (16442444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e017fc0dc182ff1d92e0a154df0525070262a2f4fa9f58bd125580e33667a154`  
		Last Modified: Thu, 01 Oct 2020 23:24:50 GMT  
		Size: 175.2 MB (175224168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
