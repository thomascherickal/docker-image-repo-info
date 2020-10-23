## `openjdk:16-ea-21-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:757089090faa7ce808610fbce7feddf8f9edf4a9219fe27362a355349beafdbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:16-ea-21-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:e5e239d616fd733ee526251cd583b34a6f8ec8ab2b05c0ae6bf9d616fcd05ce6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263479561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fb9b755826272319d637bec79929f8f42696ed2f5036ea62187e0e729740414`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 21:23:41 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Thu, 22 Oct 2020 02:16:46 GMT
ADD file:59b4b5dc4ff5144ae5143af034a90495ce3fb94b66f4966e4d06c26c73506d90 in / 
# Thu, 22 Oct 2020 02:16:47 GMT
CMD ["/bin/bash"]
# Thu, 22 Oct 2020 02:36:16 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 22 Oct 2020 02:36:16 GMT
ENV LANG=en_US.UTF-8
# Thu, 22 Oct 2020 02:36:17 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 22 Oct 2020 02:36:17 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 23:34:52 GMT
ENV JAVA_VERSION=16-ea+21
# Thu, 22 Oct 2020 23:35:06 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/21/GPL/openjdk-16-ea+21_linux-aarch64_bin.tar.gz; 			downloadSha256=bee09458526a8c10a40f3d4e5bf6c384b1bbc6f9002997d2f4c0d8c090cca1f8; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/21/GPL/openjdk-16-ea+21_linux-x64_bin.tar.gz; 			downloadSha256=3294d805c6125a6dd55a387f82f74df0c9fc0bce06934061fb3ff2dd42075b33; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 22 Oct 2020 23:35:06 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:95cb88f1fe95a86a8b517472bb2c588e7f8ec90b705f71e24ec099e3a266e9de`  
		Last Modified: Thu, 22 Oct 2020 02:18:58 GMT  
		Size: 48.2 MB (48245353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49088501182fac2779f26885b335f17d9328f05236e6de06597dd813a20dadf2`  
		Last Modified: Thu, 22 Oct 2020 02:45:34 GMT  
		Size: 16.2 MB (16228231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885ddfaf2b32df71626502363380d1b44a02571599f4d03844102d5399a5bd50`  
		Last Modified: Thu, 22 Oct 2020 23:40:35 GMT  
		Size: 199.0 MB (199005977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
