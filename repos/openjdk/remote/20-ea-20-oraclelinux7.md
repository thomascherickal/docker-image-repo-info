## `openjdk:20-ea-20-oraclelinux7`

```console
$ docker pull openjdk@sha256:4849783bed49fc62681e8cb28b128cb51afe49cf4dce29f5f1ff11bfc543d93d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-20-oraclelinux7` - linux; amd64

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

### `openjdk:20-ea-20-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:87d6ac3d31e3db6d5cd7622266d3342afa85399e8e9605bfd6e85f7cb6e6c448
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.4 MB (261362397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08aff36a027d1698517c28b30aac0005d73cecef7fd56eaf072d26713dfca779`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 21 Oct 2022 19:41:26 GMT
ADD file:4541eaa8394632e064f29982b181d348a272ef2413862ac71178a341243bce2e in / 
# Fri, 21 Oct 2022 19:41:27 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 20:06:49 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 21 Oct 2022 20:06:49 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Fri, 21 Oct 2022 20:06:50 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Oct 2022 20:06:51 GMT
ENV LANG=en_US.UTF-8
# Fri, 21 Oct 2022 20:06:52 GMT
ENV JAVA_VERSION=20-ea+20
# Fri, 21 Oct 2022 20:07:10 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='0cb0f79bee2e61134a86049952a1e572bb3e2dad49aa200a20f18c697715a402'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='4db7319dfbfb4a3561e9707c0178d0ba8d6413bc94f13d8c9ce406fd7445e000'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Oct 2022 20:07:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:76fdd4639925cb62e440f1f25d41e3d474d0afd52a63ddf021701ae8f260c928`  
		Last Modified: Fri, 21 Oct 2022 19:43:32 GMT  
		Size: 50.4 MB (50428227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217d0e0ef4d8b79b020b26a462bb9a71f35c685aa8669454c231a47cafbf70a4`  
		Last Modified: Fri, 21 Oct 2022 20:14:31 GMT  
		Size: 15.3 MB (15260410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2026436b48f419db48576123289b12c54d3a58e87b6df84d9f7e2af153574b1`  
		Last Modified: Fri, 21 Oct 2022 20:14:49 GMT  
		Size: 195.7 MB (195673760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
