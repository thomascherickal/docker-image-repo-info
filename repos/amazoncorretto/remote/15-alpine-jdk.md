## `amazoncorretto:15-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:435762204cc194628c190bd1e7ae1314d2e244b2faf42cfec1f8b0efb6183e6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3a4e2dde42bfc4d93a28aaf0e5cfc2ba0b173787fc8147601ec081228c8ea515
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207723606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:284fac6862c63db92b6b441c27f75a5797ac17bb31c65185a629588778b2ec50`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:38 GMT
ADD file:b2c067f4304d00c91fc9fd92f2e58853412cc705dfda4d1cf658fab965d5802c in / 
# Thu, 25 Mar 2021 22:19:38 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 01:59:42 GMT
ARG version=15.0.2.7.1
# Fri, 26 Mar 2021 01:59:52 GMT
# ARGS: version=15.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Fri, 26 Mar 2021 01:59:52 GMT
ENV LANG=C.UTF-8
# Fri, 26 Mar 2021 01:59:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 26 Mar 2021 01:59:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:22599d3e9e25e799b87521b94e20d20a601ffad16cf676274fdf94b089e4b979`  
		Last Modified: Thu, 25 Mar 2021 22:20:35 GMT  
		Size: 2.8 MB (2799762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc105230db47cb4483a93980f608f1d629c2bab534c153fd386eb601dcd65d4`  
		Last Modified: Fri, 26 Mar 2021 02:02:53 GMT  
		Size: 204.9 MB (204923844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
