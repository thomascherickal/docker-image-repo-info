## `amazoncorretto:17-alpine3.15-jdk`

```console
$ docker pull amazoncorretto@sha256:cb96a821c0b99415f765e565701e72ec440a5a0d5d7a5a66a65e656d8ab86315
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.15-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ff0d103d17d2f3e11415e0ec2dea57bb8e0ddf601eb3a3a8b015fc82ac0e5db2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194627048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e81fb7b3101e8518f7349940a228c1bbba848c40a495948838bbfe7fca3ba8c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 15:47:21 GMT
ARG version=17.0.2.8.1
# Wed, 23 Mar 2022 15:47:29 GMT
# ARGS: version=17.0.2.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Wed, 23 Mar 2022 15:47:29 GMT
ENV LANG=C.UTF-8
# Wed, 23 Mar 2022 15:47:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 23 Mar 2022 15:47:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982a7f30e9ffa052d687a7a580b5b159c761e9a8edc21448000795f4838b3ede`  
		Last Modified: Wed, 23 Mar 2022 15:50:54 GMT  
		Size: 191.8 MB (191814359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
