## `amazoncorretto:19-alpine3.13-jdk`

```console
$ docker pull amazoncorretto@sha256:bce86eb637aab49007a5cafa6d2e3c87426754c422d45df6605aadabe48eaf3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:19-alpine3.13-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:a16d3c55ee0fe03629d7ca1e6ad14b4f3afcfd6a0c287c0a1e418890035c4a6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.0 MB (203045630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da180ac906b2f6652accdaaa7f8a08b29ffd6a9a12ec79b9c25f9379995afad`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:14 GMT
ADD file:7fd90c097e2c4587dee91726d71abc02fa1aa6a3a3395c862206a4e14e0c299c in / 
# Tue, 09 Aug 2022 17:20:14 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:37:29 GMT
ARG version=19.0.0.36.1
# Thu, 06 Oct 2022 19:37:37 GMT
# ARGS: version=19.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-19=$version-r0
# Thu, 06 Oct 2022 19:37:38 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 19:37:38 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 06 Oct 2022 19:37:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:72cfd02ff4d01b1f319eed108b53120dea0185b916d2abeb4e6121879cbf7a65`  
		Last Modified: Tue, 09 Aug 2022 17:21:16 GMT  
		Size: 2.8 MB (2827571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7276572084160cf95057193f714b4d485d0a5f77335f10436f4fe5e6bed068e`  
		Last Modified: Thu, 06 Oct 2022 19:49:22 GMT  
		Size: 200.2 MB (200218059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
