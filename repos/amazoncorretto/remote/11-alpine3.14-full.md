## `amazoncorretto:11-alpine3.14-full`

```console
$ docker pull amazoncorretto@sha256:04cb37bd664ee53e913f20c1181b54ce7c8d0a555fded882ed20021e6e8cc6f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine3.14-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:51ccae49dde33d8b2da2c266a704fa406a311a18a5aba2617b42786cc6dd2462
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.0 MB (196039842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2fabfda944410dc5446914500e32a62f39019a8ae5110a5c5bf0763eeb8ea7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:37:44 GMT
ARG version=11.0.16.8.1
# Tue, 09 Aug 2022 17:37:50 GMT
# ARGS: version=11.0.16.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 09 Aug 2022 17:37:51 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 17:37:51 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 09 Aug 2022 17:37:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1a102cf87154eefbd2fdd37b65cfde5b83d2c66f7b337edd0e6825db5d768c`  
		Last Modified: Tue, 09 Aug 2022 17:43:26 GMT  
		Size: 193.2 MB (193212353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
