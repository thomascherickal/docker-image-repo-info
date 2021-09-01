## `amazoncorretto:11-alpine`

```console
$ docker pull amazoncorretto@sha256:c225131e21c08557e8fc67093d2d754cbcb60acd87a5b76705536a289cc0e906
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6c7d2b8ea57c59261869b9fccaf539922bee14bd0369592e33a774896b1e9e5d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196173778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44d331805194149821fc0bcd3df484be70e89bee0a11400e41d38b99b0df65b8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:50 GMT
ARG version=11.0.12.7.1
# Wed, 01 Sep 2021 00:31:00 GMT
# ARGS: version=11.0.12.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 01 Sep 2021 00:31:01 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:31:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:31:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3e805fde94ec062176cd36ed45061f412bb1e5ccd372790eb4f0f9674e0ff5`  
		Last Modified: Wed, 01 Sep 2021 00:33:22 GMT  
		Size: 193.4 MB (193372071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
