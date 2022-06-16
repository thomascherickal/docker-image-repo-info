## `openjdk:20-ea-1-oraclelinux7`

```console
$ docker pull openjdk@sha256:9d37bb5380be521bf3745f3150ceee624bdb6bb749477d8918aeabecd9d9f0b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:20-ea-1-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:a45d5d9f1272250dfa83d820338a6365be801e6bf8bedfd31a12ac6d2f16a2c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.6 MB (260557565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd3bad8141072acf3260ea467b928cd4a21d19c24c4d66284b59488ab80b71aa`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 01 Jun 2022 17:42:45 GMT
ADD file:38edee0c3395726e7b6c49418111c57515fb5158f2d9007df25b1126becbe835 in / 
# Wed, 01 Jun 2022 17:42:45 GMT
CMD ["/bin/bash"]
# Wed, 01 Jun 2022 18:06:10 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 16 Jun 2022 00:49:29 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 16 Jun 2022 00:49:30 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jun 2022 00:49:31 GMT
ENV LANG=en_US.UTF-8
# Thu, 16 Jun 2022 00:49:32 GMT
ENV JAVA_VERSION=20-ea+1
# Thu, 16 Jun 2022 00:49:49 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/1/GPL/openjdk-20-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='0abed92a0e13e5d0f0d02463a90b21a040db83ea57617f5c61c5547862152766'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/1/GPL/openjdk-20-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='898a2f8ca4e530d154e94ca685ef4f03341cd78f3514661a03c8f87bfbdd2371'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 16 Jun 2022 00:49:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f32f2fa821eee2ec9063a1b4319bd010b81853e0530a69451b35606e68be303b`  
		Last Modified: Wed, 01 Jun 2022 17:45:48 GMT  
		Size: 49.3 MB (49342882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7422ac4472668232f731f99e0cfcf6637faa083e23675a9b4fd3259163ebff4`  
		Last Modified: Wed, 01 Jun 2022 18:19:08 GMT  
		Size: 15.3 MB (15264563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb08dc83e98edb1e7759f3bac3cb5c86b52f01aaf1b52741f9f6300dc7022724`  
		Last Modified: Thu, 16 Jun 2022 01:05:04 GMT  
		Size: 196.0 MB (195950120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
