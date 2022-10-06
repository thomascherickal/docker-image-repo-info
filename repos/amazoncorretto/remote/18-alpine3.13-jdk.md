## `amazoncorretto:18-alpine3.13-jdk`

```console
$ docker pull amazoncorretto@sha256:4b53d355ea5c409a132c9449ce0b3df21c1a9c459334ad70d47524cc99d45433
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:18-alpine3.13-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e1bf834e172c20d83f11b814924ebbd48829a1281d48db868d8edf45ec603a70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195688433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f9eb7cc1a8e0f77c3ee9ed1d93e20bd4212a2519597a8d7f05caef3acbb347`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:14 GMT
ADD file:7fd90c097e2c4587dee91726d71abc02fa1aa6a3a3395c862206a4e14e0c299c in / 
# Tue, 09 Aug 2022 17:20:14 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:36:45 GMT
ARG version=18.0.2.9.1
# Thu, 06 Oct 2022 19:36:53 GMT
# ARGS: version=18.0.2.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-18=$version-r0
# Thu, 06 Oct 2022 19:36:54 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 19:36:54 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 06 Oct 2022 19:36:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:72cfd02ff4d01b1f319eed108b53120dea0185b916d2abeb4e6121879cbf7a65`  
		Last Modified: Tue, 09 Aug 2022 17:21:16 GMT  
		Size: 2.8 MB (2827571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e50c223de92d2e6ab9031beb44bdb1fd182a53c494157dc0b32485cfebf25d1`  
		Last Modified: Thu, 06 Oct 2022 19:47:17 GMT  
		Size: 192.9 MB (192860862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
