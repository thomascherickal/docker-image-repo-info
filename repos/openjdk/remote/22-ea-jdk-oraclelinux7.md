## `openjdk:22-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:d0423495c55b3aca646984e0391bc6023dd5323d894ead98a3eaade961830cdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:ab9e835d8e47ec209a9ab75031a50886f248c12b32dd1c86e4ebc8ffccdd9948
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.9 MB (269855784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b169c8888b92bf6b7e4f6487c8b1eeee5a8332d454faf531aab8bcac188d4ad`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 12 Oct 2023 21:29:07 GMT
ADD file:2726e2d5d9aaf4024ea489d9049884aa06c0c95d6111037ba29987ba029ddc44 in / 
# Thu, 12 Oct 2023 21:29:07 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 22:19:41 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 12 Oct 2023 22:19:41 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Thu, 12 Oct 2023 22:19:41 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 22:19:41 GMT
ENV LANG=en_US.UTF-8
# Thu, 12 Oct 2023 22:19:42 GMT
ENV JAVA_VERSION=22-ea+18
# Thu, 12 Oct 2023 22:19:52 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/18/GPL/openjdk-22-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='07830a4cc21745464a68057e8c441e98d4cd673cd02348e9791d9eafe9f3d0df'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/18/GPL/openjdk-22-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='03432a54970a3005c521d34b44a2438ac28f8fe150bf686e28cea6ea9b2a002e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Oct 2023 22:19:52 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9ad776bc39341b015fa96ec38b0ef30213514fedd245d657d3188d81b46d367c`  
		Last Modified: Thu, 12 Oct 2023 21:30:53 GMT  
		Size: 50.5 MB (50496653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d12b7af3f237d48ffcd0cb3d2738d9661d2029fe2ac6fb20e11ead3a56ce551`  
		Last Modified: Thu, 12 Oct 2023 22:21:35 GMT  
		Size: 14.3 MB (14251137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b4f750a67f5843fd05a73efdcf6e2b7593b449bdd4b423ff55cccd37090b11`  
		Last Modified: Thu, 12 Oct 2023 22:21:48 GMT  
		Size: 205.1 MB (205107994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f4524ba8c2ab40e434691df483927ce5d03dceb3a212a1cf8068f933aeeed4e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.7 MB (269747348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48c9e4c8831497c809c1ae3282ef4de7f61b5268117d911d6c4338edcf982655`
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
# Thu, 12 Oct 2023 15:36:18 GMT
ENV JAVA_VERSION=22-ea+18
# Thu, 12 Oct 2023 15:36:31 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/18/GPL/openjdk-22-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='07830a4cc21745464a68057e8c441e98d4cd673cd02348e9791d9eafe9f3d0df'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/18/GPL/openjdk-22-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='03432a54970a3005c521d34b44a2438ac28f8fe150bf686e28cea6ea9b2a002e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Oct 2023 15:36:33 GMT
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
	-	`sha256:4d49f55571712548d7173a054fa3559f296036ab23056e1d0e5f7ccf38460709`  
		Last Modified: Thu, 12 Oct 2023 15:38:15 GMT  
		Size: 203.4 MB (203394122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
