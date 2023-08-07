## `amazoncorretto:8-alpine3.17-jdk`

```console
$ docker pull amazoncorretto@sha256:504e570b9b2eedae2aba2a7be684b5c74a5f2530ead8e448b2f7fbf0ab4de622
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-alpine3.17-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f3ed3a97ba1b174fd8bed6f9225cccf0b3b51e850b63bdd160c9dac8e6934d6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.4 MB (103435880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e267f2332d19aaca0c5f1c9d2e87992592c98ae8f271cbb294803554f1ca6e46`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:45:27 GMT
ARG version=8.382.05.1
# Mon, 07 Aug 2023 19:45:30 GMT
# ARGS: version=8.382.05.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 19:45:31 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 19:45:31 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 19:45:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61fbff801b92cc68b709c4495cc609d98d6cad04bec9efd89a253b3158a0565`  
		Last Modified: Mon, 07 Aug 2023 19:51:20 GMT  
		Size: 100.1 MB (100057271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-alpine3.17-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:a30c656fd1c50a68f546c82b2c4ba4415d4922388b1b18e9978f38fd90a755e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103050327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6609376c72359d94f8c893886617a6a76ba23d88ae32c75772d0c3db22a6a73e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:23:19 GMT
ARG version=8.382.05.1
# Mon, 07 Aug 2023 20:23:22 GMT
# ARGS: version=8.382.05.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 20:23:23 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:23:23 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 20:23:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c21e1d99b31d66f22afe6bbdb98c873097e4f240f2568c64bf32ad7119112a`  
		Last Modified: Mon, 07 Aug 2023 20:35:49 GMT  
		Size: 99.8 MB (99792037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
