## `amazoncorretto:8u322-alpine`

```console
$ docker pull amazoncorretto@sha256:a1a4c51b882a716c3c8403a47b8a282199bfab27ba95ab8d0e1fc961be5ca301
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u322-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:4adf18a20d7bca074d9c595dbd9bd2e583edd661038076beeb0075cbe13e955c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101916030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca00cd71ece94017dc219dee56b189251d34beb7034d23746430fd02d9204ffc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 15:46:36 GMT
ARG version=8.322.06.2
# Wed, 23 Mar 2022 15:46:41 GMT
# ARGS: version=8.322.06.2
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Wed, 23 Mar 2022 15:46:41 GMT
ENV LANG=C.UTF-8
# Wed, 23 Mar 2022 15:46:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 23 Mar 2022 15:46:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d255e20c18a5e42fc58d6655c496489ec613ae96a2dd24bba4a98eceada5ea1`  
		Last Modified: Wed, 23 Mar 2022 15:49:03 GMT  
		Size: 99.1 MB (99103341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
