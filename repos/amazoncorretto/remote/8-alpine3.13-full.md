## `amazoncorretto:8-alpine3.13-full`

```console
$ docker pull amazoncorretto@sha256:3f41934b59f23d2deadcfac6e96042c50dcb77e1381a70eb499671665c2ad555
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.13-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:23a553412922bda7bbc07718717b9cb8b9d73b102210fd03cbbce5e817b250ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101611427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c86fc25e36645ea39ac5cbd0777cb01281d99e6ea0509411b9a857ed25ae704`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:26 GMT
ADD file:e15461ac94648d9599df6304a53587fc8bfceaf6e111ee5917860e95ed9e751c in / 
# Tue, 19 Jul 2022 22:20:26 GMT
CMD ["/bin/sh"]
# Fri, 29 Jul 2022 20:20:00 GMT
ARG version=8.342.07.4
# Fri, 29 Jul 2022 20:20:05 GMT
# ARGS: version=8.342.07.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Fri, 29 Jul 2022 20:20:06 GMT
ENV LANG=C.UTF-8
# Fri, 29 Jul 2022 20:20:06 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 29 Jul 2022 20:20:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:627fad6f28f79c3907ad18a4399be4d810c0e1bb503fe3712217145c555b9d2f`  
		Last Modified: Tue, 19 Jul 2022 22:21:04 GMT  
		Size: 2.8 MB (2819330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f79e84495a671ac9ac55e4b071454c2178c0c5cda90a137aa998130982ebe65`  
		Last Modified: Fri, 29 Jul 2022 20:23:08 GMT  
		Size: 98.8 MB (98792097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
