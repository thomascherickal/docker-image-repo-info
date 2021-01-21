## `amazoncorretto:8u282-alpine`

```console
$ docker pull amazoncorretto@sha256:bfe9b77d5ec4f4083cf1db58ea06c7404c193f1f7589a37073f501716e39bb7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8u282-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c816e1cf210b0638c68d0b2b2323835ccf2775eff15920c9632a89a7f19cdf45
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101783426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:578c324b3a924889de20419aa30535ec714f24223bf6cc698fbc80234a919bef`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 21 Jan 2021 19:20:18 GMT
ARG version=8.282.08.1
# Thu, 21 Jan 2021 19:20:23 GMT
# ARGS: version=8.282.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Thu, 21 Jan 2021 19:20:23 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jan 2021 19:20:23 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 21 Jan 2021 19:20:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5540e4aac0d3797e100a2625f1fe943bff0aca8b0da1330d1002097ba1155ca0`  
		Last Modified: Thu, 21 Jan 2021 19:22:30 GMT  
		Size: 99.0 MB (98984360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
