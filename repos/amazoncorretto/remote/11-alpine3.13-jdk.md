## `amazoncorretto:11-alpine3.13-jdk`

```console
$ docker pull amazoncorretto@sha256:7beb209a70f0b2316fec635bfee0c7cf4e2af7b92ae244a08f090123aa632810
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine3.13-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:531d08a4378369177270a79af213574501f9cd87603384df40429a04d7c1998b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.0 MB (196033435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07eb4ee38c7bfa432df7cd890f185c851dfce88e3334652d7f0d8d6f9bc80608`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:14 GMT
ADD file:7fd90c097e2c4587dee91726d71abc02fa1aa6a3a3395c862206a4e14e0c299c in / 
# Tue, 09 Aug 2022 17:20:14 GMT
CMD ["/bin/sh"]
# Tue, 16 Aug 2022 23:20:10 GMT
ARG version=11.0.16.9.1
# Tue, 16 Aug 2022 23:20:17 GMT
# ARGS: version=11.0.16.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 16 Aug 2022 23:20:18 GMT
ENV LANG=C.UTF-8
# Tue, 16 Aug 2022 23:20:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 16 Aug 2022 23:20:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:72cfd02ff4d01b1f319eed108b53120dea0185b916d2abeb4e6121879cbf7a65`  
		Last Modified: Tue, 09 Aug 2022 17:21:16 GMT  
		Size: 2.8 MB (2827571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aed9200f89bf36844eeba8a4599c9524f2bb368e54b002bcc11c4305eca482`  
		Last Modified: Tue, 16 Aug 2022 23:24:14 GMT  
		Size: 193.2 MB (193205864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
