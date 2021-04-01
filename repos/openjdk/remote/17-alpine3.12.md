## `openjdk:17-alpine3.12`

```console
$ docker pull openjdk@sha256:2b45fdb0cc7863a243154db4119ceaab6dff3d40f30a60c5f8539784ad92de55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:17-alpine3.12` - linux; amd64

```console
$ docker pull openjdk@sha256:0280ccaca79ca83df41f01cb43b56a57ed4038936a4b3cbe55f469fe1ac85057
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.5 MB (190525133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44dff9a33d395c6f2a3c32b30efa9a014355999b591ab0c109d94fd386242543`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:15:27 GMT
RUN apk add --no-cache java-cacerts
# Thu, 01 Apr 2021 01:15:27 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Thu, 01 Apr 2021 01:15:27 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Apr 2021 01:15:27 GMT
ENV JAVA_VERSION=17-ea+14
# Thu, 01 Apr 2021 01:15:49 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/14/binaries/openjdk-17-ea+14_linux-x64-musl_bin.tar.gz'; 			downloadSha256='f07a1ac921333dafac1cd886ad49600ce143be7efebd32e1a02599a8a0829dd4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 01 Apr 2021 01:15:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4354a9508ff15b9e1bfdc60a073f2c25564fb52dca39dd9127f6e79767a848b`  
		Last Modified: Thu, 01 Apr 2021 01:22:00 GMT  
		Size: 927.4 KB (927394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfe3fcc9ce7a61e6add0ee16235d5c2f37e996e1aa45c001ecc21fa68400c3d`  
		Last Modified: Thu, 01 Apr 2021 01:22:21 GMT  
		Size: 186.8 MB (186798027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
