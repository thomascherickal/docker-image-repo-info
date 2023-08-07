## `amazoncorretto:20-alpine3.17`

```console
$ docker pull amazoncorretto@sha256:bce873ced42e2538fc6af5b5c844428a83cb38a9f35c78b6a5cb39dabfc21877
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-alpine3.17` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:82b8777993ceebb0cbb56f56c8a52f15c6e5dd4f8427e105b2543f66d1c431fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.0 MB (157953602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5fa243a59547f86fc37760f176fb141a67ff5973f36a7e7b6aac265bd89a1dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:48:03 GMT
ARG version=20.0.2.9.1
# Mon, 07 Aug 2023 19:48:10 GMT
# ARGS: version=20.0.2.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0 &&     rm -rf /usr/lib/jvm/java-20-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 19:48:10 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 19:48:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 19:48:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f680cf01f4f75025410a248a6d6540db0801af0eacd1add438f6d72084050665`  
		Last Modified: Mon, 07 Aug 2023 19:57:46 GMT  
		Size: 154.6 MB (154574993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e84dc0b65a273f978e4ae2852f55f633c53449aea91a9762c2e54d5000e8e996
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155919672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067705161c072dc7253d274c250e3aa295470e309e8c61c07cd0361b218156c9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:31:25 GMT
ARG version=20.0.2.9.1
# Mon, 07 Aug 2023 20:31:30 GMT
# ARGS: version=20.0.2.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0 &&     rm -rf /usr/lib/jvm/java-20-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 20:31:32 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:31:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 20:31:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6246ba14829c5e8a1d80cab237bbc39b5c6d920a946683a2b00a85d04c1046`  
		Last Modified: Mon, 07 Aug 2023 20:47:23 GMT  
		Size: 152.7 MB (152661382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
