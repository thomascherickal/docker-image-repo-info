## `amazoncorretto:8u392-alpine3.17`

```console
$ docker pull amazoncorretto@sha256:37db670287aa0c266923323199a6fe4aeb8587d9e4a1f93c01300baf50c5f7f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u392-alpine3.17` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:fdd55733662210d90136f4198c6697934ce1c5537aaf5aa17ed000643335de63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.4 MB (103439537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69ed6746038680075365ae3a72d33717c3b8c93b8484b0bba76b9bfc0c544ecc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 03:17:41 GMT
ARG version=8.392.08.1
# Thu, 19 Oct 2023 03:17:45 GMT
# ARGS: version=8.392.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Thu, 19 Oct 2023 03:17:45 GMT
ENV LANG=C.UTF-8
# Thu, 19 Oct 2023 03:17:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 19 Oct 2023 03:17:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31d51a25fd4445e326c230832ddf4068fe2cc1a8fcf853ad06c81419bf8a78c`  
		Last Modified: Thu, 19 Oct 2023 03:34:12 GMT  
		Size: 100.1 MB (100060928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u392-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:79aa1709e129f28e7c2a0344e253e8c6ff2f58ae27e8c45797db31421a5f6dce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103063771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24450bbaadac15dcf390132658437847d3304a39da9206ac6e6e2c7af3b7afc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:07 GMT
ADD file:e5c66967d6570e36da50c9d42dd8f8f55e6c6a65b92c79601ea9e750c076fa2a in / 
# Thu, 30 Nov 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:44:47 GMT
ARG version=8.392.08.1
# Fri, 01 Dec 2023 02:44:54 GMT
# ARGS: version=8.392.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Fri, 01 Dec 2023 02:44:55 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 02:44:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 01 Dec 2023 02:44:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:b8180c93b172865af87a7c0e7e3c8bcb139e0d0c92e19c96467ff2cd4c8919ad`  
		Last Modified: Thu, 30 Nov 2023 23:11:45 GMT  
		Size: 3.3 MB (3258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2303ac8083678caa97c4a2893305e349a2fcfe71470c4846449cd2af6af63e37`  
		Last Modified: Fri, 01 Dec 2023 02:49:04 GMT  
		Size: 99.8 MB (99805423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
