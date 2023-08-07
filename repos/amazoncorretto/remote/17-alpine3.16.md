## `amazoncorretto:17-alpine3.16`

```console
$ docker pull amazoncorretto@sha256:7fcbc3a00216257c32929cb1061abc24593e398c808e832a6f81b1db79bc9b03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-alpine3.16` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5c565cf73e54c5cdcfb392dd169343d3821910679a39e53d2d02818df5d6b9e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.5 MB (148545625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb90c9a83d014483206d3d7692824dd11a33df2237d323107b9b8d9a2cb6209a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:47:12 GMT
ARG version=17.0.8.7.1
# Mon, 07 Aug 2023 19:47:17 GMT
# ARGS: version=17.0.8.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0 &&     rm -rf /usr/lib/jvm/java-17-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 19:47:17 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 19:47:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 19:47:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c039e2d71a6d5ca575312c543e683b07786cc120cfe16e4ad738df29b6af44`  
		Last Modified: Mon, 07 Aug 2023 19:55:24 GMT  
		Size: 145.7 MB (145737942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:20f659a9310b6463d5ca408d3b7e1772d12a8fdd553953440db5603d1a0fd735
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146843802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c46019aa2f7f6c6358185deb128b08b82ea99bc7f29122d7e7a3aedc99f48b6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:29:51 GMT
ARG version=17.0.8.7.1
# Mon, 07 Aug 2023 20:29:55 GMT
# ARGS: version=17.0.8.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0 &&     rm -rf /usr/lib/jvm/java-17-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 20:29:57 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:29:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 20:29:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18770e11742a0f3677839d193780ab5ede5da446bf1c4c9ef608b6f5dcc9db5e`  
		Last Modified: Mon, 07 Aug 2023 20:44:07 GMT  
		Size: 144.1 MB (144135779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
