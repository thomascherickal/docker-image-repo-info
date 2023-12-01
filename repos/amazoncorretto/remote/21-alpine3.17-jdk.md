## `amazoncorretto:21-alpine3.17-jdk`

```console
$ docker pull amazoncorretto@sha256:6f2afc98fca258172ceed520301b2edab45e80b7f6fee46c469bf79709d7eea5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:21-alpine3.17-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:05c79d58a093e0140f227c9f1306393932ae75cfacad52f665e90442797b94a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162591813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d074d7151b56e92735ea4d15a21772bc47aa383ffc2c97c3fc368e9a41a69026`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 03:28:28 GMT
ARG version=21.0.1.12.1
# Thu, 19 Oct 2023 03:28:34 GMT
# ARGS: version=21.0.1.12.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-21=$version-r0 &&     rm -rf /usr/lib/jvm/java-21-amazon-corretto/lib/src.zip
# Thu, 19 Oct 2023 03:28:35 GMT
ENV LANG=C.UTF-8
# Thu, 19 Oct 2023 03:28:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 19 Oct 2023 03:28:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f283ad7db92a13e09a661352c8b31bdfd86b8bdcd3e187a0a3908708db1459b1`  
		Last Modified: Thu, 19 Oct 2023 03:46:53 GMT  
		Size: 159.2 MB (159213204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:21-alpine3.17-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:f2e842e96d19c2e9f3a50fa9d50471e4cb46c05718026637a07641dda8cf403e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.5 MB (160454001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5ad5a763e51bbd81ec12347f28506a74783a5824d9fce5126c1c46da0ce82cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:07 GMT
ADD file:e5c66967d6570e36da50c9d42dd8f8f55e6c6a65b92c79601ea9e750c076fa2a in / 
# Thu, 30 Nov 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:47:02 GMT
ARG version=21.0.1.12.1
# Fri, 01 Dec 2023 02:47:10 GMT
# ARGS: version=21.0.1.12.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-21=$version-r0 &&     rm -rf /usr/lib/jvm/java-21-amazon-corretto/lib/src.zip
# Fri, 01 Dec 2023 02:47:12 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 02:47:12 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 01 Dec 2023 02:47:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:b8180c93b172865af87a7c0e7e3c8bcb139e0d0c92e19c96467ff2cd4c8919ad`  
		Last Modified: Thu, 30 Nov 2023 23:11:45 GMT  
		Size: 3.3 MB (3258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539306a3734ab5d610dcdb760e44580e4cdaf6f9f42984fbb6854d2d123b91d9`  
		Last Modified: Fri, 01 Dec 2023 02:53:20 GMT  
		Size: 157.2 MB (157195653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
