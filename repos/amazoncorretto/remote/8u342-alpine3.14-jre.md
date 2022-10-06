## `amazoncorretto:8u342-alpine3.14-jre`

```console
$ docker pull amazoncorretto@sha256:eb4e89b439e98e45899a9d2e10fa3e70c2c1e264de23187f66bf39e3cd66d00e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u342-alpine3.14-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:23adabc3d03f1a1241821dddcf34c8429a0d22831b3ab5e284f276e1180b73ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43267033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae5a39e8c3032c31d99a9fee26a59a2c2e5ac7b77c0851d91365faf26931c3e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:34:40 GMT
ARG version=8.342.07.4
# Thu, 06 Oct 2022 19:34:50 GMT
# ARGS: version=8.342.07.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Thu, 06 Oct 2022 19:34:50 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 19:34:50 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0df49d531c05a4ec09ff38d87cb70265749d89ca441215e1305c5b5532531ea`  
		Last Modified: Thu, 06 Oct 2022 19:41:16 GMT  
		Size: 40.4 MB (40439544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
