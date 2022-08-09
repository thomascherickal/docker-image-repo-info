## `amazoncorretto:17-alpine3.13-full`

```console
$ docker pull amazoncorretto@sha256:8640ade02842ea86e48e1ecfdd4a7b9780537265813c8b2c9ffbbe4552ef22fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.13-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3527645fe648b7769e8cce65f6a3baba811ee1363b9baefbd4eedea6597d7e2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194489251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51eb77231c03997057912f4e4d986ff179cb986047b06e827529b9abeff4d754`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:14 GMT
ADD file:7fd90c097e2c4587dee91726d71abc02fa1aa6a3a3395c862206a4e14e0c299c in / 
# Tue, 09 Aug 2022 17:20:14 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:06 GMT
ARG version=17.0.4.8.1
# Tue, 09 Aug 2022 17:38:14 GMT
# ARGS: version=17.0.4.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Tue, 09 Aug 2022 17:38:14 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 17:38:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 09 Aug 2022 17:38:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:72cfd02ff4d01b1f319eed108b53120dea0185b916d2abeb4e6121879cbf7a65`  
		Last Modified: Tue, 09 Aug 2022 17:21:16 GMT  
		Size: 2.8 MB (2827571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1f42922444fdc0c498e302baf42650a75dad71dc1b5d942d90262c4cd7dde3`  
		Last Modified: Tue, 09 Aug 2022 17:44:34 GMT  
		Size: 191.7 MB (191661680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
