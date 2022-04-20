## `amazoncorretto:8-alpine3.14-jre`

```console
$ docker pull amazoncorretto@sha256:207a20f1d71bda7592743b882c1d73e6a5377b2c4d30d26c443b8870afffa215
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.14-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:1d9161f5b2b92f39850281cd44780284e59271ecc06fdc81313d559bac99d47f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43226182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24b88f05cfc536f0fc4e58deaed68a1ee8dbba5c8cb1822a2e57dd027fc15e3a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 22:23:20 GMT
ARG version=8.332.08.1
# Tue, 19 Apr 2022 22:23:30 GMT
# ARGS: version=8.332.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Tue, 19 Apr 2022 22:23:31 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:23:31 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36c8d1a33a7c237db73dbad4be085b7b4cb2414938ba7e2df5dd358de6b37fe`  
		Last Modified: Tue, 19 Apr 2022 22:31:14 GMT  
		Size: 40.4 MB (40407812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
