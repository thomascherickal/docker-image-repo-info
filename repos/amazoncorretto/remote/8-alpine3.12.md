## `amazoncorretto:8-alpine3.12`

```console
$ docker pull amazoncorretto@sha256:999e2b7f9279e0f260329b67bfae43cc994e88d691f7bc96e2d455d67030f1e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.12` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d0450e2743c8ae7b546387eb747fe27ff28caa6a700a2053b68b7d9d0a787573
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101833069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ceb59abcee83c29f6388844aac2c9745ba11c877e94aa4a1e2dd829000ed8c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:26 GMT
ARG version=8.302.08.1
# Wed, 01 Sep 2021 00:30:33 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 01 Sep 2021 00:30:34 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:30:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:30:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d34235dfe864bd38e7376e34561b8d34096f5870b751c61514b43013316a413`  
		Last Modified: Wed, 01 Sep 2021 00:32:33 GMT  
		Size: 99.0 MB (99031362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
