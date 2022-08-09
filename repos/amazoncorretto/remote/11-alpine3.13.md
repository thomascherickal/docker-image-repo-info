## `amazoncorretto:11-alpine3.13`

```console
$ docker pull amazoncorretto@sha256:785cb6472d8828f019ff2afbb3447374661921fe7a971b21202819045347f367
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine3.13` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e3c73b10f1e325ee1e7bfd218e63f16e8a393d539983768246fcfcb2b487bbdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.0 MB (196037039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:908184e185040c66a006d68a9788dfdb7403412218eb61879dcefad205bc01f6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:14 GMT
ADD file:7fd90c097e2c4587dee91726d71abc02fa1aa6a3a3395c862206a4e14e0c299c in / 
# Tue, 09 Aug 2022 17:20:14 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:37:33 GMT
ARG version=11.0.16.8.1
# Tue, 09 Aug 2022 17:37:40 GMT
# ARGS: version=11.0.16.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 09 Aug 2022 17:37:41 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 17:37:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 09 Aug 2022 17:37:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:72cfd02ff4d01b1f319eed108b53120dea0185b916d2abeb4e6121879cbf7a65`  
		Last Modified: Tue, 09 Aug 2022 17:21:16 GMT  
		Size: 2.8 MB (2827571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f559a78cb02da29af0fd09fc561b6be8cda50f741b7fe4b78333eaf30d2808`  
		Last Modified: Tue, 09 Aug 2022 17:42:58 GMT  
		Size: 193.2 MB (193209468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
