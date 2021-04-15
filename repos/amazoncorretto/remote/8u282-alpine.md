## `amazoncorretto:8u282-alpine`

```console
$ docker pull amazoncorretto@sha256:6fe5342eff1d74d0f1e7767e072ae1da760b891280ff7dbd8600f6a2dde4ef30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8u282-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d95a540c69bfd15ffa7ced13d8190e0549edaa3f29dc4b0a70414166d6d1cafb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101784983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae5c0ee01475d4ca4a2d4a77616aae01268d6577c36068556cbd51dc5678ec0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:38:39 GMT
ARG version=8.282.08.1
# Wed, 14 Apr 2021 19:38:43 GMT
# ARGS: version=8.282.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 14 Apr 2021 19:38:44 GMT
ENV LANG=C.UTF-8
# Wed, 14 Apr 2021 19:38:44 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 14 Apr 2021 19:38:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1039621ac19611846de8a7be112221b0ca2e47451f80478a85c3d93b517235`  
		Last Modified: Wed, 14 Apr 2021 19:41:12 GMT  
		Size: 99.0 MB (98984416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
