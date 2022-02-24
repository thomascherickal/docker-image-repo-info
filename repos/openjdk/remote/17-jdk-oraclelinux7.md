## `openjdk:17-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:d6a8df9edbe48a38d76be42dc426a4411fc9ec7e1aa2a5d1ac9ed285c9a910f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:cccf7275458f68ec83acb6628cda68f43b1badbef51cbd9bcc1dc81d285c0811
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.3 MB (251259791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a74cffa8774744fa544a72a7f560e0ead9922f990c520a75f3bd861df9b293`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Feb 2022 01:15:28 GMT
ADD file:a953cc04974b35909ddbd8826601c0824f8cc920ebc522046d4ca64e69c2c26f in / 
# Thu, 24 Feb 2022 01:15:29 GMT
CMD ["/bin/bash"]
# Thu, 24 Feb 2022 01:47:39 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 24 Feb 2022 01:49:15 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Thu, 24 Feb 2022 01:49:15 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Feb 2022 01:49:15 GMT
ENV LANG=en_US.UTF-8
# Thu, 24 Feb 2022 01:49:15 GMT
ENV JAVA_VERSION=17.0.2
# Thu, 24 Feb 2022 01:49:27 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 24 Feb 2022 01:49:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5269884ada0dd8683c910050c7cf3a447be8fcb9f733519f759745b117b217cc`  
		Last Modified: Thu, 24 Feb 2022 01:16:17 GMT  
		Size: 48.3 MB (48331243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48833246028b375ed9389617e9b863bfab004c27db95b93b1e8b7c646ce3f9a1`  
		Last Modified: Thu, 24 Feb 2022 01:58:10 GMT  
		Size: 15.4 MB (15402391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a54d32a5e6eaf716ba7442e6c4f30579bf7fea46fb33dfd5b53667d779ccd7`  
		Last Modified: Thu, 24 Feb 2022 02:00:11 GMT  
		Size: 187.5 MB (187526157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:6add62f50105186daecde69f37c71544480252894b4ed707a375807c02742c1d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.7 MB (251711144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c246d3a9df8c9f7fd60cf058bd14c88bb6748e42236b2a236f62d3846a200711`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Feb 2022 01:19:51 GMT
ADD file:c293ee454f68e84cb645f758fa6566a1eb9e75fb5a28101eab9f1cafd97e9226 in / 
# Thu, 24 Feb 2022 01:19:52 GMT
CMD ["/bin/bash"]
# Thu, 24 Feb 2022 02:04:47 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 24 Feb 2022 02:06:59 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Thu, 24 Feb 2022 02:07:00 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Feb 2022 02:07:01 GMT
ENV LANG=en_US.UTF-8
# Thu, 24 Feb 2022 02:07:02 GMT
ENV JAVA_VERSION=17.0.2
# Thu, 24 Feb 2022 02:07:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='0022753d0cceecacdd3a795dd4cea2bd7ffdf9dc06e22ffd1be98411742fbb44'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.2/dfd4a8d0985749f896bed50d7138ee7f/8/GPL/openjdk-17.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='13bfd976acf8803f862e82c7113fb0e9311ca5458b1decaef8a09ffd91119fa4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 24 Feb 2022 02:07:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4402421e0ca8a48b128ce814a1f5f26684df2d5f1caf1afa1ffbb8fabccdf603`  
		Last Modified: Thu, 24 Feb 2022 01:20:47 GMT  
		Size: 48.9 MB (48902111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7e8a0b0254507322b36a7a006c588143e280eb30aeb748e6245570ea648cb7`  
		Last Modified: Thu, 24 Feb 2022 02:21:23 GMT  
		Size: 16.4 MB (16444983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87683ad552c4b14f72d6585c85a27176cafaa7b5cfd043f92abeb1023d45de9f`  
		Last Modified: Thu, 24 Feb 2022 02:23:30 GMT  
		Size: 186.4 MB (186364050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
