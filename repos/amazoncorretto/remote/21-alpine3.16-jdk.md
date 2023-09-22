## `amazoncorretto:21-alpine3.16-jdk`

```console
$ docker pull amazoncorretto@sha256:28579a958edeb3d3b319f4a6338a8541ef9fceaacb5b417cd223405cbe71257e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:21-alpine3.16-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d7d3d3f7206190176dbf5bacff4886a383e6892b7b92841046d16e64be2e2f0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.0 MB (161993279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db399712ec369899ab644cc6c71326516a72cdd2e08c3d6acaaa7b1156f357bf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Fri, 22 Sep 2023 00:23:24 GMT
ARG version=21.0.0.35.1
# Fri, 22 Sep 2023 00:23:30 GMT
# ARGS: version=21.0.0.35.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-21=$version-r0 &&     rm -rf /usr/lib/jvm/java-21-amazon-corretto/lib/src.zip
# Fri, 22 Sep 2023 00:23:31 GMT
ENV LANG=C.UTF-8
# Fri, 22 Sep 2023 00:23:31 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 22 Sep 2023 00:23:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353d490cd0e4ad7c278e4fac612043d51a367b1342f59831777bc8fc501b687e`  
		Last Modified: Fri, 22 Sep 2023 00:28:57 GMT  
		Size: 159.2 MB (159185596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:21-alpine3.16-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:bd437b5604ee6f493fbfd792f528ca1af8cfb87daafeed42968c3008d23c105f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.9 MB (159875453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:241989b6640b22a2d7fe61e945fcf30c6dda1276a3a0c231bf4cb4006cd46c21`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Fri, 22 Sep 2023 00:43:36 GMT
ARG version=21.0.0.35.1
# Fri, 22 Sep 2023 00:43:41 GMT
# ARGS: version=21.0.0.35.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-21=$version-r0 &&     rm -rf /usr/lib/jvm/java-21-amazon-corretto/lib/src.zip
# Fri, 22 Sep 2023 00:43:43 GMT
ENV LANG=C.UTF-8
# Fri, 22 Sep 2023 00:43:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 22 Sep 2023 00:43:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a2f4effcd816b4c358687145c5dfb7665868bd18973297492e4293c2b77446`  
		Last Modified: Fri, 22 Sep 2023 00:48:27 GMT  
		Size: 157.2 MB (157167430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
