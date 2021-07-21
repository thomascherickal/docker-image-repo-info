## `amazoncorretto:8u302-alpine`

```console
$ docker pull amazoncorretto@sha256:b97cd4e1f357a3d445db6d1566838a6c91b312cea4085ecc791370ac288860d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u302-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4edb6c988dbd6611a208f16ec06ee915289808745e32fe27691026a64519229d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101831898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93854338cb3296eb3934ba3706b7ce61dcf904607e3f9fd4139583c5aa4739bb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:20:54 GMT
ARG version=8.302.08.1
# Wed, 21 Jul 2021 00:21:00 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 21 Jul 2021 00:21:00 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 21 Jul 2021 00:21:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f141ea8c2ff0050b64f199d6c95d96fef7a0e9f7daac05c2ff20af6a7e0f25`  
		Last Modified: Wed, 21 Jul 2021 00:23:11 GMT  
		Size: 99.0 MB (99031331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
