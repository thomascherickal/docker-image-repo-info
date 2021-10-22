## `openjdk:18-ea-20-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:1f8d9db10817f01c06a2fac5bd762501f7c06cfca5ae03b3554d0a537ea1a777
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:18-ea-20-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:a3146e0a13171c3575d6d130a255f31491a4451551ea57635940aa753dbe1a99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243529775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:868c1183ffd0f6e5978b04a7abb565219d9009b463ba777add30a2f78292a261`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 13 Oct 2021 18:29:51 GMT
ADD file:3223e5829b65b376c23e1faa6f519d37b0166b38063f91b793a8ed710a39fe33 in / 
# Wed, 13 Oct 2021 18:29:51 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 18:47:48 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 13 Oct 2021 18:47:48 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 13 Oct 2021 18:47:48 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 18:47:49 GMT
ENV LANG=C.UTF-8
# Thu, 21 Oct 2021 23:40:48 GMT
ENV JAVA_VERSION=18-ea+20
# Thu, 21 Oct 2021 23:41:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='aa609b9f3a4a31b3cb3649a39dabf11476d9c5f1f3b8b9583b2be48e14e3c321'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='a1bfee1fed3794347cfce38d0f4a163b7e90702ceb5fe9256d06664c0daa5726'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 21 Oct 2021 23:41:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:58c4eaffce77ac1fb013bf82c91927c631802ad54465ebc9b687b5dc8ee73c02`  
		Last Modified: Wed, 13 Oct 2021 18:31:20 GMT  
		Size: 42.0 MB (41961111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a22c806ee8aa2b360bd5818a4f78bc3da280abb86f3db09805b1daddd78324`  
		Last Modified: Wed, 13 Oct 2021 18:56:49 GMT  
		Size: 13.5 MB (13489427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d5999e95a024c93652a115a00230bdb890f472297e0d18734729e689804ae2`  
		Last Modified: Thu, 21 Oct 2021 23:52:34 GMT  
		Size: 188.1 MB (188079237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
