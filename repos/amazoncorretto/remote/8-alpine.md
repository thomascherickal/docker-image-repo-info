## `amazoncorretto:8-alpine`

```console
$ docker pull amazoncorretto@sha256:755b765a6eaebac4917e85729602d52ce04ef92e0fb3e97a2cbe644f8f193752
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:0d8fb5af4921c06953dbf07d473b8a138c28c2ed008102505049f322db0e56a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101859334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba5bc5a94d9b82426874bd9ee436cbf3c1856480f68f338513ba06e9ae75248a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 20 Oct 2021 18:19:52 GMT
ARG version=8.312.07.1
# Wed, 20 Oct 2021 18:19:56 GMT
# ARGS: version=8.312.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 20 Oct 2021 18:19:57 GMT
ENV LANG=C.UTF-8
# Wed, 20 Oct 2021 18:19:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 20 Oct 2021 18:19:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7defde508fc6e60971c2c5ed5ed91fb39b2641ae1896dbd69d1aff88680487`  
		Last Modified: Wed, 20 Oct 2021 18:23:50 GMT  
		Size: 99.1 MB (99057627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
