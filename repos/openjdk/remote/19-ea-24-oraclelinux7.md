## `openjdk:19-ea-24-oraclelinux7`

```console
$ docker pull openjdk@sha256:f1f85f418eb96babbe927e056a9ef102d242f5262603d76fcd0d0b1831238ef1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-24-oraclelinux7` - linux; amd64

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

### `openjdk:19-ea-24-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:cd7f1919150eef86fc2f1ee3abac88a5821ef85715b3efe93bb15e65d7ebb915
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.2 MB (259184032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30f97f3264ba6c5f340d7f7fcb9841bd5d79fceb04873b5c4b7a8a7ec0b39376`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 01 Jun 2022 17:42:45 GMT
ADD file:38edee0c3395726e7b6c49418111c57515fb5158f2d9007df25b1126becbe835 in / 
# Wed, 01 Jun 2022 17:42:45 GMT
CMD ["/bin/bash"]
# Wed, 01 Jun 2022 18:06:10 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 01 Jun 2022 18:06:10 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Wed, 01 Jun 2022 18:06:11 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Jun 2022 18:06:12 GMT
ENV LANG=en_US.UTF-8
# Wed, 01 Jun 2022 18:06:13 GMT
ENV JAVA_VERSION=19-ea+24
# Wed, 01 Jun 2022 18:06:33 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/24/GPL/openjdk-19-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='3f7b2351ee42bc75d9200072d7fd241fcbd9accd60983a245cd005531723e051'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/24/GPL/openjdk-19-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='baa4ad8447e5d179e22d269a8a9f653b86173df964fef78c95aef5c2ca902b7a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 01 Jun 2022 18:06:34 GMT
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
	-	`sha256:12310eaa76dc0b607136c0aa7d7f6cabc9c42882574b952e59239eb7f5928f31`  
		Last Modified: Wed, 01 Jun 2022 18:19:35 GMT  
		Size: 194.6 MB (194576587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
