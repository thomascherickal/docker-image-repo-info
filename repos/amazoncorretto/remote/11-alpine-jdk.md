## `amazoncorretto:11-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:425c4a06c339c0daafd93d553ed274bfd6bde0df94693f111655aebb31898f98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:dc61008163572cf3d92e94e09b987fa8753520687d93f3d0b07d318827c05c8f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195688657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4193c28ed9bafd6b9ac969d9c212ce9141c87f7ff3bf8efc8336877ff6311f2e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 22:24:42 GMT
ARG version=11.0.15.9.1
# Tue, 19 Apr 2022 22:24:48 GMT
# ARGS: version=11.0.15.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 19 Apr 2022 22:24:49 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:24:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Apr 2022 22:24:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488151d00693d39310ffbe2c5d010922714e008ba04718d255fabf2fc43218df`  
		Last Modified: Tue, 19 Apr 2022 22:34:20 GMT  
		Size: 192.9 MB (192874098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
