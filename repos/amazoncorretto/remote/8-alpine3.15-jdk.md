## `amazoncorretto:8-alpine3.15-jdk`

```console
$ docker pull amazoncorretto@sha256:13e9763b10df2f0fc5f2ba92d6b6ce9378526fdf4ed00fb9115c24e776533ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-alpine3.15-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:badc9eb8c7787c4fb5c0e9859082e31b9e9cf67fe9ea79e17ed9d0b9b8fb6f6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102883295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d05969e9bc6197b0a884726b700633f1dbb18505d8acd596f9562e9cee5dbd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:45:00 GMT
ARG version=8.382.05.1
# Mon, 07 Aug 2023 19:45:04 GMT
# ARGS: version=8.382.05.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 19:45:05 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 19:45:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 19:45:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100ec18cef0fdce64f12ac23cec01fc7a48991ca9a946abf6c480dbabbd66994`  
		Last Modified: Mon, 07 Aug 2023 19:50:08 GMT  
		Size: 100.1 MB (100057289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-alpine3.15-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:2395fd29ab5263c59cdc917d239a8d6c8556f4a2e8006ee727907bc1b7cd7dec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102512395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2543dfa50d61569a1f5c84f2b41e0be3e9e473648abaa77de51bab252510a74c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:22:56 GMT
ARG version=8.382.05.1
# Mon, 07 Aug 2023 20:23:00 GMT
# ARGS: version=8.382.05.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 20:23:01 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:23:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 20:23:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b97ccd6a6a79213b7e73db1e43e067893436f6887e1ed0c694101a7deea230b`  
		Last Modified: Mon, 07 Aug 2023 20:34:36 GMT  
		Size: 99.8 MB (99791527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
