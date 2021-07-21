## `amazoncorretto:8-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:2c978d2e5921d10abf49c845a2a46b502544c15e2ca733d7b552b350aa691068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ff95ea78ce154abaa581bf382295bacf13c0474357ef144fcd96ac1d6d5e851d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43148477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7543a33c551dd671bf563addcbfbf76cc5a3020d86a8479847202e8bd0b5dce1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 21 Jul 2021 00:20:54 GMT
ARG version=8.302.08.1
# Wed, 21 Jul 2021 00:21:07 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 21 Jul 2021 00:21:07 GMT
ENV LANG=C.UTF-8
# Wed, 21 Jul 2021 00:21:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be776a268f00c1a39cc8385fff8b6582ba6d26a76a929e1f13dbdf0208d73520`  
		Last Modified: Wed, 21 Jul 2021 00:23:31 GMT  
		Size: 40.3 MB (40347910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
