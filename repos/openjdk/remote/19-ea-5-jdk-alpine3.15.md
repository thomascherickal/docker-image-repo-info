## `openjdk:19-ea-5-jdk-alpine3.15`

```console
$ docker pull openjdk@sha256:b96a2c957a61e5bf413d5ed6305bdbe1fc3fcb9e0cd5a5a04a432baaacc27b92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:19-ea-5-jdk-alpine3.15` - linux; amd64

```console
$ docker pull openjdk@sha256:739477cf4a7acdc668f348ed53b74a97bc5769de75029d3477f4d34bfaa77ae8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.3 MB (194324089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e7077992b1be5c0ae7d5c0adcfd20d1ebf52db14f1629f49bb3981a0e75a86`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 17:17:58 GMT
RUN apk add --no-cache java-cacerts
# Wed, 23 Mar 2022 17:17:58 GMT
ENV JAVA_HOME=/opt/openjdk-19
# Wed, 23 Mar 2022 17:17:58 GMT
ENV PATH=/opt/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 17:17:58 GMT
ENV JAVA_VERSION=19-ea+5
# Wed, 23 Mar 2022 17:18:23 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/5/binaries/openjdk-19-ea+5_linux-x64-musl_bin.tar.gz'; 			downloadSha256='0ee67a41fe97341f131bd4f065ed6092d55c15de5f00f8ba1e57d21eefb2c787'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 23 Mar 2022 17:18:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69ef1ecbd183501e60a2f2d77ac0dfc0cce0aad98559de5dc3264f90c9c8cb2`  
		Last Modified: Wed, 23 Mar 2022 17:24:22 GMT  
		Size: 918.6 KB (918571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b15f3030896b3da0b09bd1151138a08c6c8efd3260da822bb3378f0a362cdfe`  
		Last Modified: Wed, 23 Mar 2022 17:24:36 GMT  
		Size: 190.6 MB (190592829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
