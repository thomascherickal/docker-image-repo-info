## `amazoncorretto:11-alpine-full`

```console
$ docker pull amazoncorretto@sha256:bf0a361478158b40d3592ab1cdc8b9c63640e13e22524cecc4805e85039eb565
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e84fdbf13c8bba52e28de9f845a1fc30866fdf6bba1ff942e35f4c00023991ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196172744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8720e708cea9fc900fd3b0997cad3aa9c4f11da06801c1ee0e235f2fc730ea4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:21:10 GMT
ARG version=11.0.12.7.1
# Wed, 21 Jul 2021 00:21:17 GMT
# ARGS: version=11.0.12.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 21 Jul 2021 00:21:17 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 21 Jul 2021 00:21:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477fef7b3b9fb84dc86e1350700f7c6dfcee763129bea71c593cd7de0c9d516`  
		Last Modified: Wed, 21 Jul 2021 00:23:55 GMT  
		Size: 193.4 MB (193372177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
