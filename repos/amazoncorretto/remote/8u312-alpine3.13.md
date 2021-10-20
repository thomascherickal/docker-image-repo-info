## `amazoncorretto:8u312-alpine3.13`

```console
$ docker pull amazoncorretto@sha256:8588b317d25405340fa1c8e1b9972865aca993af80fa01b7b073a64051c6d762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u312-alpine3.13` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:43b9df14c4ce4dc18da12b92704077fac73f86436bbe41000d5a970df7d1385a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101872085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c15a575eb69705b46c99ef65ecc53e3892e3a0290563a9ce3061d574e857f3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 20 Oct 2021 18:20:06 GMT
ARG version=8.312.07.1
# Wed, 20 Oct 2021 18:20:10 GMT
# ARGS: version=8.312.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 20 Oct 2021 18:20:10 GMT
ENV LANG=C.UTF-8
# Wed, 20 Oct 2021 18:20:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 20 Oct 2021 18:20:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074778edee736add0b45fe83b159ab7f0635d9c6f1ca31b4276e8973ed8bbb34`  
		Last Modified: Wed, 20 Oct 2021 18:24:39 GMT  
		Size: 99.1 MB (99058006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
