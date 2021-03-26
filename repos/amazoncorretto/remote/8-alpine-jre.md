## `amazoncorretto:8-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:a23867ac09ff44cd0a12eadc7b04dabf3fa5426ecdcc21fbe430f90852a04395
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:12c06f0d634b03374eb6c7876a503b9e5d77da91bdb1d401259fac75c1c06509
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43115748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42c2e48c59c15ff17d4f3061ec18152fa3daaa050d48542ee894818bccf15531`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:11 GMT
ARG version=8.282.08.1
# Fri, 26 Mar 2021 01:59:24 GMT
# ARGS: version=8.282.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Fri, 26 Mar 2021 01:59:24 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65cc8853ab18e84a7be865c72f2b25f59f3723f3a3ce5943d4680aa16d59fc2`  
		Last Modified: Fri, 26 Mar 2021 02:01:43 GMT  
		Size: 40.3 MB (40315986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
