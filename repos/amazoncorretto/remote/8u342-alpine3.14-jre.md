## `amazoncorretto:8u342-alpine3.14-jre`

```console
$ docker pull amazoncorretto@sha256:28f1e5570f922a85278bada816f36617860941de4e7dc5f056199e288419af60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u342-alpine3.14-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:9fa5b0ab611916081a054aafa33b8731548b81fe402572be2a0ab920435444c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43266968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97d4bf9865033579ce5597f0690962ffc3fad359b0684d62f65ec8cb24ac88e7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:37:00 GMT
ARG version=8.342.07.4
# Tue, 09 Aug 2022 17:37:14 GMT
# ARGS: version=8.342.07.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Tue, 09 Aug 2022 17:37:14 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 17:37:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9791446884627df00fab3c908ebe178d644df015bff062d53ff92241309184`  
		Last Modified: Tue, 09 Aug 2022 17:41:42 GMT  
		Size: 40.4 MB (40439479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
