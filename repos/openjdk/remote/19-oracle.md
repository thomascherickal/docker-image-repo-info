## `openjdk:19-oracle`

```console
$ docker pull openjdk@sha256:afcee14c3c3f24943419d176eb41f078a00292bc2384d70fde62cc23d3f2ada1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:290a47f33c538d654bef0ce0654dce6f8bb31da376730a4e21c22f273fce0505
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248906613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a51e8216de928d5f4180e8af95539490685d366e1349cfb7a635087bc3805718`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:35:27 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:35:57 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 04 Aug 2022 01:35:57 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 01:35:57 GMT
ENV LANG=C.UTF-8
# Thu, 04 Aug 2022 01:35:57 GMT
ENV JAVA_VERSION=19-ea+33
# Thu, 04 Aug 2022 01:36:08 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='31aa1cf0a266dfc90d9e85d688379a2b2b9b1888bb7df326a4434dc92fdc105f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='8e758bdc4cd496f29c85a53ce1eb155b7ee8f945c11517cc4a766492349c52e2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 04 Aug 2022 01:36:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d72ac1fb23a36f89addf60367990f28d5c0882e4b8f569c77b51c51eb271261`  
		Last Modified: Thu, 04 Aug 2022 01:42:41 GMT  
		Size: 13.5 MB (13506500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee7b165b9a710a0b807e1c823e7137ac4b20c0233a2a338568b2989c5160f33`  
		Last Modified: Thu, 04 Aug 2022 01:43:56 GMT  
		Size: 196.2 MB (196176161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:254620db0c4eeb5361fdedd7bef07ce809a5341834aab842785b83bbd0b9be3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.3 MB (247318666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:964cc7af85f1f6cb4ce24aecd75aa3e4aea74d9e06dae0620bb269d887998770`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:01:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:02:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 04 Aug 2022 01:02:12 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 01:02:13 GMT
ENV LANG=C.UTF-8
# Thu, 04 Aug 2022 01:02:14 GMT
ENV JAVA_VERSION=19-ea+33
# Thu, 04 Aug 2022 01:02:26 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='31aa1cf0a266dfc90d9e85d688379a2b2b9b1888bb7df326a4434dc92fdc105f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='8e758bdc4cd496f29c85a53ce1eb155b7ee8f945c11517cc4a766492349c52e2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 04 Aug 2022 01:02:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e225b6ab834ff85ee0d347a2859ecb14fc169f362360408133589ab8a37d8333`  
		Last Modified: Thu, 04 Aug 2022 01:14:59 GMT  
		Size: 14.3 MB (14278746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f700a0e6a3f9c22240890cdc06cd1bea5730b3db16db23efe9a23838b033c7a`  
		Last Modified: Thu, 04 Aug 2022 01:16:42 GMT  
		Size: 195.0 MB (195016874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
