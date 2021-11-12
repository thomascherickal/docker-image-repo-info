## `amazoncorretto:17-alpine3.14`

```console
$ docker pull amazoncorretto@sha256:08ef1f1a94af2a34e27d1d933cafa09a58acc416ccf6f5539d4d7ffa882d52a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.14` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ff8ce3c4125ec3da58f2dc2bb3847d0d2bcd14b18678a3b45a3849d14267f49b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194589484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11983e6629417c4b5b001494e742a3065cc7521143db633c86ee9f5ea8ec9abd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:20:20 GMT
ARG version=17.0.1.12.1
# Fri, 12 Nov 2021 21:20:31 GMT
# ARGS: version=17.0.1.12.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Fri, 12 Nov 2021 21:20:31 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:20:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 12 Nov 2021 21:20:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9d30db1130d95f2b294a5134eaa3057b5420a4d5579d84c8bf85214f1f543f`  
		Last Modified: Fri, 12 Nov 2021 21:28:06 GMT  
		Size: 191.8 MB (191766503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
