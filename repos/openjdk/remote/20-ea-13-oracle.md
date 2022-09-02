## `openjdk:20-ea-13-oracle`

```console
$ docker pull openjdk@sha256:32c8ec4a81d3b689b5667800562e175e25ff6597c4bd4ee8c112bdd6553faa3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:20-ea-13-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:42ddb992452f7339ada07b673bf8a57a0224fed700b73f387d33259a69a4e876
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248940168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01336e47f34cb058b887d72fcf5471c9d48108437239251e05e37f39b9b7e721`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 30 Aug 2022 21:20:34 GMT
ADD file:94f0ad5f0805806df710f02659592b7a0ee14643d54d40f0dca144e16c2c69ec in / 
# Tue, 30 Aug 2022 21:20:34 GMT
CMD ["/bin/bash"]
# Tue, 30 Aug 2022 21:47:35 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 30 Aug 2022 21:47:35 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Tue, 30 Aug 2022 21:47:35 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Aug 2022 21:47:35 GMT
ENV LANG=C.UTF-8
# Thu, 01 Sep 2022 23:28:48 GMT
ENV JAVA_VERSION=20-ea+13
# Thu, 01 Sep 2022 23:29:11 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/13/GPL/openjdk-20-ea+13_linux-x64_bin.tar.gz'; 			downloadSha256='93758735b85b0f9e8a98728ad636942bcf266476824286754fe6dbd2a2f6aeff'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/13/GPL/openjdk-20-ea+13_linux-aarch64_bin.tar.gz'; 			downloadSha256='305cd60ab947992620abe377f9d1fe876c6a80db3fab369a8cb5517edbfc30be'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 01 Sep 2022 23:29:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:492d84e496ea03370b8fb5b989ff003b89c51a2f037216835b8b3f93dcc4d405`  
		Last Modified: Tue, 30 Aug 2022 21:21:33 GMT  
		Size: 39.5 MB (39521774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d74542bd1abb51e0ea04904a65559d263d7f85b016fcbd81a65768553957ae`  
		Last Modified: Tue, 30 Aug 2022 21:51:36 GMT  
		Size: 12.2 MB (12240649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dfe48da11470c247fa981273c806df609902ffe35aeeabcf10e087cb6c96a0`  
		Last Modified: Thu, 01 Sep 2022 23:34:19 GMT  
		Size: 197.2 MB (197177745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
