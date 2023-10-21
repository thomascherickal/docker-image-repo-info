## `openjdk:22-ea-20-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:d291f4698117f6a61ba5de4db580dacc0c7e6eaed9e85504cfb5a19b2952e2fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:22-ea-20-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:dd4bda98605a33e77d26296ab5c72f0fc25fd11343fc5d6b5dc3bc31f7816ad2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.8 MB (269832514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:340b87851f60b8e5dee843d804bf21e0681a87ebf7973265149be4d83f6269ce`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 12 Oct 2023 11:00:59 GMT
ADD file:67e4d2ca8c1a10f2e3e0b8cbfac921504e96756141f9a105cd73ccf06d7f1a70 in / 
# Thu, 12 Oct 2023 11:01:00 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 15:36:18 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 12 Oct 2023 15:36:18 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Thu, 12 Oct 2023 15:36:18 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 15:36:18 GMT
ENV LANG=en_US.UTF-8
# Fri, 20 Oct 2023 23:58:39 GMT
ENV JAVA_VERSION=22-ea+20
# Fri, 20 Oct 2023 23:58:52 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/20/GPL/openjdk-22-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='5f1627efa81951307900954bbf7b2e49d8c5303615cf116959c273e9707b0496'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/20/GPL/openjdk-22-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='8fa022a3b05cc606bccbb014baea9e821954a789ba40b6fd39b40cd4453fb9f5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 20 Oct 2023 23:58:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:71a92edb27cabcf1cd98fcea78da305dc7a1e70eb00b95534f57518084cf9823`  
		Last Modified: Thu, 12 Oct 2023 11:02:30 GMT  
		Size: 51.1 MB (51108085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd1aca6ce046cb2bd184372ec5ea080c5717e57b0cca639c9419105820a0922`  
		Last Modified: Thu, 12 Oct 2023 15:38:01 GMT  
		Size: 15.2 MB (15245141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df523810eb0e86a805b90c6f81b3d5c9aea16e395a4d7f42030a0e517a704cb9`  
		Last Modified: Sat, 21 Oct 2023 00:04:34 GMT  
		Size: 203.5 MB (203479288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
