## `amazoncorretto:18-alpine3.12-jdk`

```console
$ docker pull amazoncorretto@sha256:1cf8d6c63fe76bf54cec36553f25142f6a47b0262dde516b5db1ddd35c093c4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:18-alpine3.12-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:67fbef53e71f5427819758a679b2b06ce12bcb353136d5466c617719018c8464
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.8 MB (195770157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c5b7cca044131d5e4411693017c82a6749daa9b6d2a540b4660156c84976e8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:19 GMT
ADD file:c1aa87a3b464fca64d769444b5201bc0426a1f517c91c4a7916270e10f8b300b in / 
# Tue, 05 Apr 2022 00:20:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 22:26:46 GMT
ARG version=18.0.1.10.1
# Tue, 19 Apr 2022 22:26:52 GMT
# ARGS: version=18.0.1.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-18=$version-r0
# Tue, 19 Apr 2022 22:26:52 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:26:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Apr 2022 22:26:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:1b7ca6aea1ddfe716f3694edb811ab35114db9e93f3ce38d7dab6b4d9270cb0c`  
		Last Modified: Tue, 05 Apr 2022 00:21:10 GMT  
		Size: 2.8 MB (2808060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6330e7f32162878daff41dbee243c6584eb696ab4cb2cb2490f1b1add4ca10`  
		Last Modified: Tue, 19 Apr 2022 22:38:04 GMT  
		Size: 193.0 MB (192962097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
