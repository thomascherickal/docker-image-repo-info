## `amazoncorretto:11-alpine3.12-jdk`

```console
$ docker pull amazoncorretto@sha256:8c1e57d72bd4efb25d54d13fae65f9c22e58a09c84fa76c685e1c4d974987c6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine3.12-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5f1dda70bd3880670fc53056a6847a92a13e8450524d4ce25fa4f9fc80160978
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196124533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efb00c90cb3e7100783f33dbd9cc00e392d3b7315c3c217d7811698e5f036f37`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 20 Oct 2021 18:21:00 GMT
ARG version=11.0.13.8.1
# Wed, 20 Oct 2021 18:21:05 GMT
# ARGS: version=11.0.13.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 20 Oct 2021 18:21:06 GMT
ENV LANG=C.UTF-8
# Wed, 20 Oct 2021 18:21:06 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 20 Oct 2021 18:21:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272ee1342cdea6659a3b4fdc8e91e09a988b31dce1178118a89df96af342cd33`  
		Last Modified: Wed, 20 Oct 2021 18:26:26 GMT  
		Size: 193.3 MB (193322826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
