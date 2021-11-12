## `amazoncorretto:8-alpine3.14`

```console
$ docker pull amazoncorretto@sha256:49dfb41021d56b081065f9aff21bc50b4a21f106aaa0d8d681b81fd058c7bd6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.14` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:61e77e03f0d8da8e4fc30ad80c00b6ab0d925227d0ad808938667093c88c608f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101876014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3915310176e556e8cbe1f0bc7aa57c19c95c1a26d7b15e59852006489706c94`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:18:58 GMT
ARG version=8.312.07.1
# Fri, 12 Nov 2021 21:19:02 GMT
# ARGS: version=8.312.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Fri, 12 Nov 2021 21:19:03 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:19:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 12 Nov 2021 21:19:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcef2a039d917672bf97be286896f076800b69fdee0bad2b264eeb3e2921ce3`  
		Last Modified: Fri, 12 Nov 2021 21:24:14 GMT  
		Size: 99.1 MB (99053033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
