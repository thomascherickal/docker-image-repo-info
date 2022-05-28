## `openjdk:19-oraclelinux7`

```console
$ docker pull openjdk@sha256:33084526fa53beeea8c5fffa2749f7496324a9cd19b142eac29443d99d88deaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:54e2dfb9d5953023ab894e7b9e5e4d1df588a8c2133e775bd393c1d9c4940230
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.7 MB (258693785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c1260d7624e4f84c3325a4087c105245a2746cb2bb7cb1a9669ce1393cff5f`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 19 May 2022 18:21:17 GMT
ADD file:60c2a17c0433d95caf7d6bac5520da02174f48bf0c50f6f369b00bf8f9774f82 in / 
# Thu, 19 May 2022 18:21:17 GMT
CMD ["/bin/bash"]
# Thu, 19 May 2022 18:22:53 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 19 May 2022 18:22:54 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 19 May 2022 18:22:54 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 May 2022 18:22:54 GMT
ENV LANG=en_US.UTF-8
# Sat, 28 May 2022 02:16:02 GMT
ENV JAVA_VERSION=19-ea+24
# Sat, 28 May 2022 02:16:12 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/24/GPL/openjdk-19-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='3f7b2351ee42bc75d9200072d7fd241fcbd9accd60983a245cd005531723e051'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/24/GPL/openjdk-19-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='baa4ad8447e5d179e22d269a8a9f653b86173df964fef78c95aef5c2ca902b7a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 28 May 2022 02:16:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f0182e2fe516824cf8f93b207b7c4b65d05c48db476f53312b17b5cd952bfcc3`  
		Last Modified: Thu, 19 May 2022 18:22:04 GMT  
		Size: 48.8 MB (48757934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf5bd358537747774933b2ee9c613076ddeadddfb40f451054ba3989a4b2a80`  
		Last Modified: Thu, 19 May 2022 18:29:27 GMT  
		Size: 14.2 MB (14244311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff712862dd2a083b5e67977729a736074b58e1c220888e6c699c20cabf40cf1d`  
		Last Modified: Sat, 28 May 2022 02:26:49 GMT  
		Size: 195.7 MB (195691540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:384876e818bd814624c563ade16b64570c6e9ae78abcbbc8d64778b51e41327b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.2 MB (259182712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de261df67fafab1ec21455a9ee7afaa99e17559ec82a237fc8d8e207c0391f22`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 19 May 2022 17:55:42 GMT
ADD file:3d80a0730bc69825f18f411b67d8e8a6eb5b2450223ab171cf3f4f7f8b43d021 in / 
# Thu, 19 May 2022 17:55:44 GMT
CMD ["/bin/bash"]
# Thu, 19 May 2022 19:04:26 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 19 May 2022 19:04:27 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 19 May 2022 19:04:28 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 May 2022 19:04:29 GMT
ENV LANG=en_US.UTF-8
# Sat, 28 May 2022 01:36:04 GMT
ENV JAVA_VERSION=19-ea+24
# Sat, 28 May 2022 01:36:24 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/24/GPL/openjdk-19-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='3f7b2351ee42bc75d9200072d7fd241fcbd9accd60983a245cd005531723e051'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/24/GPL/openjdk-19-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='baa4ad8447e5d179e22d269a8a9f653b86173df964fef78c95aef5c2ca902b7a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 28 May 2022 01:36:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9932f90ce40726b220e1a83ec69eaecb5ceec5409d33a736f6189de512eac36e`  
		Last Modified: Thu, 19 May 2022 17:56:42 GMT  
		Size: 49.3 MB (49337178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aa262ef1f7aae5da5cd2e580c02388ffbd2dc26b81fb14478c79b9074c22a3`  
		Last Modified: Thu, 19 May 2022 19:16:45 GMT  
		Size: 15.3 MB (15268963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64ec4b324bbc09d2330e521f744b584d719e25791a42a254580213ae598ad98`  
		Last Modified: Sat, 28 May 2022 01:53:33 GMT  
		Size: 194.6 MB (194576571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
