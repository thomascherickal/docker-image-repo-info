## `amazoncorretto:11-alpine3.17`

```console
$ docker pull amazoncorretto@sha256:6cd583ce5c97bb854307185ca6589873724063bdce3e125ac3df247a4b7047cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-alpine3.17` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ede0f0ffcc66fb2d3cc845a864f7b41b2a789589d152894c85b09591201d1926
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.8 MB (144845817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:013383ebd1874a8777f24e368167d95f785812f7342da26cd993cbbdb7703a96`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 03:21:38 GMT
ARG version=11.0.21.9.1
# Thu, 19 Oct 2023 03:21:44 GMT
# ARGS: version=11.0.21.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0 &&     rm -rf /usr/lib/jvm/java-11-amazon-corretto/lib/src.zip
# Thu, 19 Oct 2023 03:21:45 GMT
ENV LANG=C.UTF-8
# Thu, 19 Oct 2023 03:21:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 19 Oct 2023 03:21:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f397b9dfe01033906d278d27bcd79a446692068aee4d8965dc587cd275153dc`  
		Last Modified: Thu, 19 Oct 2023 03:38:46 GMT  
		Size: 141.5 MB (141467208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:baa99b25cc449cc2a08c5ce706c8e7a2ca73ac70f0a301078953f79b92dd4390
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.0 MB (143002140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e356f5f19e7b4a399bf7582eec09433440d3ffc2934689ad2efb90bd8867698`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:07 GMT
ADD file:e5c66967d6570e36da50c9d42dd8f8f55e6c6a65b92c79601ea9e750c076fa2a in / 
# Thu, 30 Nov 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:45:41 GMT
ARG version=11.0.21.9.1
# Fri, 01 Dec 2023 02:45:46 GMT
# ARGS: version=11.0.21.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0 &&     rm -rf /usr/lib/jvm/java-11-amazon-corretto/lib/src.zip
# Fri, 01 Dec 2023 02:45:47 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 02:45:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 01 Dec 2023 02:45:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:b8180c93b172865af87a7c0e7e3c8bcb139e0d0c92e19c96467ff2cd4c8919ad`  
		Last Modified: Thu, 30 Nov 2023 23:11:45 GMT  
		Size: 3.3 MB (3258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe19a81fe936beb797b6ff891327e86e3d95174b0cfe07a634f6470426af1c1`  
		Last Modified: Fri, 01 Dec 2023 02:50:43 GMT  
		Size: 139.7 MB (139743792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
