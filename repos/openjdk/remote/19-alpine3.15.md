## `openjdk:19-alpine3.15`

```console
$ docker pull openjdk@sha256:14913687cbfa0892b11f0d9bf7a6c12c29cd79949a0302506b93ddb0e296e665
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:19-alpine3.15` - linux; amd64

```console
$ docker pull openjdk@sha256:d3e93ea6492fda4f9fcbeec428f321ef9b518f118f6d4edd185979231ab05160
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.3 MB (194324026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa88b26f9b3e8d88385a2cbcccd4a0e9d0d6978f65383db406db956fd2d59843`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:09:32 GMT
RUN apk add --no-cache java-cacerts
# Thu, 17 Mar 2022 18:09:32 GMT
ENV JAVA_HOME=/opt/openjdk-19
# Thu, 17 Mar 2022 18:09:32 GMT
ENV PATH=/opt/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 18:09:32 GMT
ENV JAVA_VERSION=19-ea+5
# Thu, 17 Mar 2022 18:09:44 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/5/binaries/openjdk-19-ea+5_linux-x64-musl_bin.tar.gz'; 			downloadSha256='0ee67a41fe97341f131bd4f065ed6092d55c15de5f00f8ba1e57d21eefb2c787'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Mar 2022 18:09:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95bfa6190a5f1e660dfa661cfeacb195395e181263c1cccbc3920ee6ca80bbd`  
		Last Modified: Thu, 17 Mar 2022 18:26:15 GMT  
		Size: 918.6 KB (918586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79afb24595e792b2b9730c2c5afe2d3318709911a025123e55d49e217ce392f1`  
		Last Modified: Thu, 17 Mar 2022 18:26:30 GMT  
		Size: 190.6 MB (190592804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
