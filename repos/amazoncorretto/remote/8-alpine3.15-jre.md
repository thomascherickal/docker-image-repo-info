## `amazoncorretto:8-alpine3.15-jre`

```console
$ docker pull amazoncorretto@sha256:e02c97739155cbd21c6b43107682c8c247f12d8b6840b962dccdf792ab96c551
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-alpine3.15-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:dce6c34ad61b2f7298c228dc1ef200cbb961287a0bc6d3cf5650c10811012e9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44345198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2528eb964434b50758c92cbcec2e37e72a67ca1de9edb21ac8a44b47bd5d954`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:34:18 GMT
ARG version=8.372.07.1
# Thu, 15 Jun 2023 05:34:30 GMT
# ARGS: version=8.372.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Thu, 15 Jun 2023 05:34:30 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 05:34:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd74871da25c6267ceeffc015e35e03695a1a9620c849a316525e3f2ef3fe08`  
		Last Modified: Thu, 15 Jun 2023 05:38:27 GMT  
		Size: 41.5 MB (41519282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-alpine3.15-jre` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:68123d1c407cf8eee492d7e2cddb368b22f15cf132b00adddb081521f3d1e39d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43986047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b82466e1c8376da646f042dde90eea8e65e1904118cb0e09a3133c61988a4f8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:07:45 GMT
ARG version=8.372.07.1
# Wed, 14 Jun 2023 22:07:56 GMT
# ARGS: version=8.372.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 14 Jun 2023 22:07:56 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jun 2023 22:07:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2de8f9dbc52fdb20ea919c5d0ba655bb70ada88b89949ed2a5db5ee2a994eb`  
		Last Modified: Wed, 14 Jun 2023 22:11:36 GMT  
		Size: 41.3 MB (41265246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
