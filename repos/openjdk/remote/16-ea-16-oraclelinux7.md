## `openjdk:16-ea-16-oraclelinux7`

```console
$ docker pull openjdk@sha256:8ad2282b7ec8d248eccfab58334cb58b5deceb2760dbc1138360f1aef238c9c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:16-ea-16-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:d814e3dfb77d5d4f5c100fbb4da8dae88acea00cdaeda6e36678645ce4a8308b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (261006439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:002f2ceb7c0ce2f363b1f14aef03c01d3d8208c8c438df616f32ee39d598880d`
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
# Thu, 17 Sep 2020 23:30:49 GMT
ENV JAVA_VERSION=16-ea+16
# Thu, 17 Sep 2020 23:31:01 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/16/GPL/openjdk-16-ea+16_linux-aarch64_bin.tar.gz; 			downloadSha256=6ed6f286820b9989bb460491294379eb0ec7cd689412b22151046d14ffe828be; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/16/GPL/openjdk-16-ea+16_linux-x64_bin.tar.gz; 			downloadSha256=7c57d737cded2e81487401049e9c49d505dbcfe1bc752d5ac0ee1fb8bdc611b3; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Sep 2020 23:31:01 GMT
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
	-	`sha256:c2dd77a2bbf9fc8b519ad100b722bd487c169124c83f5b766ddadacf09c64124`  
		Last Modified: Thu, 17 Sep 2020 23:35:15 GMT  
		Size: 196.8 MB (196804367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
