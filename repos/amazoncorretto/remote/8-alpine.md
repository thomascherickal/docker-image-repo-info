## `amazoncorretto:8-alpine`

```console
$ docker pull amazoncorretto@sha256:9a482474fd3b479ca9e76b56299a1a8bb90b1438f00db394e8b3e8046d1e395c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5d8fa137aaafbdaa949dc14710411d0117e7c0a773bdb17a6cbfa2f9326af9d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101784206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac15e1627ba64d9fa78a26b62d555c17485222b12da4380da9233b436382ba`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:11 GMT
ARG version=8.282.08.1
# Fri, 26 Mar 2021 01:59:17 GMT
# ARGS: version=8.282.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Fri, 26 Mar 2021 01:59:18 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c445d315c10961d8ec4eae05e42c6f61168f5806b2a44a35ba2b9f6a1f5df59`  
		Last Modified: Fri, 26 Mar 2021 02:01:22 GMT  
		Size: 99.0 MB (98984444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
