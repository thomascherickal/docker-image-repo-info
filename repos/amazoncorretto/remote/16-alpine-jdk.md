## `amazoncorretto:16-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:fa4aaa068bcb659092d836a36080c8da9b7cc28c0e5ccbb1ecc1a25706a1989b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:16-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6478e1bbcc0c13ca6c73d1b122f2f760980b448eecd6d31ddb86afea15f22cff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212400760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0263244e745216bfae352f3293932be87f975cf93cb49d68de9fca59c24eb49`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:39:39 GMT
ARG version=16.0.0.36.1
# Wed, 14 Apr 2021 19:39:53 GMT
# ARGS: version=16.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Wed, 14 Apr 2021 19:39:54 GMT
ENV LANG=C.UTF-8
# Wed, 14 Apr 2021 19:39:54 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 14 Apr 2021 19:39:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240fae9bac2160bd70d1d98ae6dd69b458cb399d5dbe8e12bf6781a6b95a1346`  
		Last Modified: Wed, 14 Apr 2021 19:43:38 GMT  
		Size: 209.6 MB (209600193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
