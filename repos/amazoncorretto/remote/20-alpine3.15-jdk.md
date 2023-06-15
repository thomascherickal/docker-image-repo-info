## `amazoncorretto:20-alpine3.15-jdk`

```console
$ docker pull amazoncorretto@sha256:d0c39fe97851ae3918f544c6bc4ac4a25a09f6e4274bc3623d656affca1235ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-alpine3.15-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1e0dd7c71d6476f59dc586c8a07b0c5101e40718181de1c5d42efdb3c6fb7731
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.5 MB (206450552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a62196fe8e8edffd125ad8fa0253f74675cb1714b1f3673b4aa47f056914370`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:36:26 GMT
ARG version=20.0.1.9.1
# Thu, 15 Jun 2023 05:36:39 GMT
# ARGS: version=20.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0
# Thu, 15 Jun 2023 05:36:40 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 05:36:40 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 15 Jun 2023 05:36:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63868b740b44d08a8d4b6ab31d468ff1003d78c113333b6e57074114f3a18d8d`  
		Last Modified: Thu, 15 Jun 2023 05:43:02 GMT  
		Size: 203.6 MB (203624636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-alpine3.15-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:741b4aa7e464b49ade37e2d3f31125e9bf4f0b47ca849e75c389e53886d1ad8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.5 MB (204452626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d88a6bceb7b9d797a834c83f6e5289511ca85bf86e6a185247adc67b15be70d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:09:35 GMT
ARG version=20.0.1.9.1
# Wed, 14 Jun 2023 22:09:43 GMT
# ARGS: version=20.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0
# Wed, 14 Jun 2023 22:09:45 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jun 2023 22:09:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 14 Jun 2023 22:09:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc394b81f9ca9723b971d51c36c9717a0ea3beb5eba2f21ea60fa93c7f9b543e`  
		Last Modified: Wed, 14 Jun 2023 22:15:57 GMT  
		Size: 201.7 MB (201731825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
