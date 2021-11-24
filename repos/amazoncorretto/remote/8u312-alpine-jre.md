## `amazoncorretto:8u312-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:003b6c580eca0fe91f7e6ee2bc83eb236c29f9c08a5b871ea57ebd0aa297df49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u312-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:213d83a5bec33b4f7d6735449b2fef0537f217f21d41c2686a6bae78e163bf37
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43184145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6521df2da8474e939b23dde33ce80be6184799a9f048f885a3f284aeabec1c6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:18:58 GMT
ARG version=8.312.07.1
# Fri, 12 Nov 2021 21:19:09 GMT
# ARGS: version=8.312.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Fri, 12 Nov 2021 21:19:09 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:19:09 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17de2cf62f67c44572e11095b0c822490b018034ae0b5a55161caf7566875bc6`  
		Last Modified: Fri, 12 Nov 2021 21:24:37 GMT  
		Size: 40.4 MB (40361164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
