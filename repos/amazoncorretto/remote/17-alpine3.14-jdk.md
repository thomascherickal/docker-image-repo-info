## `amazoncorretto:17-alpine3.14-jdk`

```console
$ docker pull amazoncorretto@sha256:29a105cfa4d51865d9fa78d0a534fb85c1a9a8bbc569a03ec19d0dd4bc1deb48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.14-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:2884d447ab06d857c7e527a1cfe34cec21b7bdea94995fd963fce286e41e646b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194489579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e81faaafc4b81e647bb98bc94803f95beb82fa01e0606ee3568b74c5ae978f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 16 Aug 2022 23:21:26 GMT
ARG version=17.0.4.9.1
# Tue, 16 Aug 2022 23:21:33 GMT
# ARGS: version=17.0.4.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Tue, 16 Aug 2022 23:21:33 GMT
ENV LANG=C.UTF-8
# Tue, 16 Aug 2022 23:21:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 16 Aug 2022 23:21:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea57a860837b7cc2f44f5edd15cd089761e452c533d956406a305d822c03eea`  
		Last Modified: Tue, 16 Aug 2022 23:26:46 GMT  
		Size: 191.7 MB (191662090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
