## `openjdk:20-ea-20-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:f0399c7e56d588c23ccf850919572807e36d5570713944206700714071433ca5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-20-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:7d93ab572eeaccfdc0b12c7df5e378564a8c46a4ed5b509bd9efbd722e761fad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261216392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe9b14c046e51dbad05d5b4b0e01dd7eb3eed304e80e8239e008f79842b51ec3`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 21 Oct 2022 19:21:18 GMT
ADD file:33b52c7a287bb91adb106cbb8b7e7bd3d38684f4aa9d19b7ef1f1af5e7288aa3 in / 
# Fri, 21 Oct 2022 19:21:18 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:52:01 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 21 Oct 2022 19:52:02 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Fri, 21 Oct 2022 19:52:02 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2022 19:52:02 GMT
ENV LANG=en_US.UTF-8
# Fri, 21 Oct 2022 19:52:02 GMT
ENV JAVA_VERSION=20-ea+20
# Fri, 21 Oct 2022 19:52:12 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='0cb0f79bee2e61134a86049952a1e572bb3e2dad49aa200a20f18c697715a402'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='4db7319dfbfb4a3561e9707c0178d0ba8d6413bc94f13d8c9ce406fd7445e000'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Oct 2022 19:52:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c19d5474d2cf2e83fc2be2ee3116c33e32d707b2ca5688ce2b086a0c318e62bd`  
		Last Modified: Fri, 21 Oct 2022 19:23:18 GMT  
		Size: 49.9 MB (49856127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561046153e09b63218385e349097fc3f08c52087f7f0f58e33ab03ff6e3046`  
		Last Modified: Fri, 21 Oct 2022 19:56:06 GMT  
		Size: 14.2 MB (14242346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e677f70502fcddc4680972d00036f2d1f0794c87e7a6cc51e604256da79e269d`  
		Last Modified: Fri, 21 Oct 2022 19:56:19 GMT  
		Size: 197.1 MB (197117919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-20-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:287eaeaa5e20fc61e3ca3ea33d0ea76f085ea121b41ef5e198bd3574fee7116a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.4 MB (261368269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57120606becb85e0aa63b2e8fe51367e2062bfb47e8d6a2507c84327959be122`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 27 Oct 2022 17:48:21 GMT
ADD file:4541eaa8394632e064f29982b181d348a272ef2413862ac71178a341243bce2e in / 
# Thu, 27 Oct 2022 17:48:21 GMT
CMD ["/bin/bash"]
# Thu, 27 Oct 2022 18:10:22 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 27 Oct 2022 18:10:23 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 27 Oct 2022 18:10:23 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Oct 2022 18:10:23 GMT
ENV LANG=en_US.UTF-8
# Thu, 27 Oct 2022 18:10:23 GMT
ENV JAVA_VERSION=20-ea+20
# Thu, 27 Oct 2022 18:10:34 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='0cb0f79bee2e61134a86049952a1e572bb3e2dad49aa200a20f18c697715a402'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='4db7319dfbfb4a3561e9707c0178d0ba8d6413bc94f13d8c9ce406fd7445e000'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 27 Oct 2022 18:10:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:76fdd4639925cb62e440f1f25d41e3d474d0afd52a63ddf021701ae8f260c928`  
		Last Modified: Fri, 21 Oct 2022 19:43:32 GMT  
		Size: 50.4 MB (50428227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e45151ebef28f688647370e198dfa565d8ff11cb7f067f0621fdf420ab3c09`  
		Last Modified: Thu, 27 Oct 2022 18:14:43 GMT  
		Size: 15.3 MB (15263621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304438c4c77a45283c13eb8cee225fdc135b227671dd33dda5a47432a82e2cce`  
		Last Modified: Thu, 27 Oct 2022 18:14:53 GMT  
		Size: 195.7 MB (195676421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
