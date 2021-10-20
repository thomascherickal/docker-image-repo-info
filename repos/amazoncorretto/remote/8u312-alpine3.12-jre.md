## `amazoncorretto:8u312-alpine3.12-jre`

```console
$ docker pull amazoncorretto@sha256:9372b8e2c2f5ab77090659755d9e62ed6dc9c65f7559c9ec36917a0ede596ff0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u312-alpine3.12-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:a0d0f26f30d88579a2f61e764dbdc7b4c012b4dc5be7b77fdc15db5b7e95a33f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43152716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26e6c60ae2213981e4dbec66960e8522a95b1ece80a270da0bd6c3474eb83cee`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 20 Oct 2021 18:19:52 GMT
ARG version=8.312.07.1
# Wed, 20 Oct 2021 18:20:03 GMT
# ARGS: version=8.312.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 20 Oct 2021 18:20:03 GMT
ENV LANG=C.UTF-8
# Wed, 20 Oct 2021 18:20:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437a5af9ed15e4d6413fbcd996ee3c915c51afa5c4e3a0addb7b15f098aa13da`  
		Last Modified: Wed, 20 Oct 2021 18:24:18 GMT  
		Size: 40.4 MB (40351009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
