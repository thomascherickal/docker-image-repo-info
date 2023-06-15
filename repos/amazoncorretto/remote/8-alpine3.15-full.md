## `amazoncorretto:8-alpine3.15-full`

```console
$ docker pull amazoncorretto@sha256:87ea2be42d3d123383df99ae297a7570a09fb6e2a0a5ea8b6edda90c2d44a5ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-alpine3.15-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:74db19db15a77c4089114ef91603197ba9c84271a0a6da66a11ee53abd6b23e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102857177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8837ccbca292166c491a620db071d66ba3062785a5c4bda343b2673d7adbeb0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:34:18 GMT
ARG version=8.372.07.1
# Thu, 15 Jun 2023 05:34:23 GMT
# ARGS: version=8.372.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Thu, 15 Jun 2023 05:34:24 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 05:34:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 15 Jun 2023 05:34:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78fe694f2aee1823959df732a03963cc518e19d1a687b672f90fc7b54298957`  
		Last Modified: Thu, 15 Jun 2023 05:38:10 GMT  
		Size: 100.0 MB (100031261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-alpine3.15-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:716389b00f6052f0ecc2aec52415c6b1e279dfbd9ec25c5a306f7c030e696880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102490847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff939dc7fc71092990c9a9ed880696b673e7df9e0acd3f19727b7be51745ade`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:07:45 GMT
ARG version=8.372.07.1
# Wed, 14 Jun 2023 22:07:50 GMT
# ARGS: version=8.372.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 14 Jun 2023 22:07:52 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jun 2023 22:07:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 14 Jun 2023 22:07:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a56f5679b9a882094f4477ba0b3bbcd6d48751bdca75ac69e011975744dc18`  
		Last Modified: Wed, 14 Jun 2023 22:11:21 GMT  
		Size: 99.8 MB (99770046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
