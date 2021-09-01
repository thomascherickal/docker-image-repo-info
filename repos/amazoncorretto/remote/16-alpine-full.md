## `amazoncorretto:16-alpine-full`

```console
$ docker pull amazoncorretto@sha256:3ba7ea36df85e9a00e428aca3cbf1d77aace7d135de555e9533a5a40db7ef707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:16-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:67f6a2dc5ae8bf75bd6ee5af504a9de65e6a32c2989f1a7ba0d5543c8c94b238
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.5 MB (212454350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e0d9c5ca59bd0e46cc3968299511a805f34b32bc066019289d5fb484c893160`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:31:11 GMT
ARG version=16.0.2.7.1
# Wed, 01 Sep 2021 00:31:23 GMT
# ARGS: version=16.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Wed, 01 Sep 2021 00:31:24 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:31:24 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 01 Sep 2021 00:31:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e812a6b7beb13efdcc4765fefd7b00d8d9868aaaa70990ea919d8a7a447682ba`  
		Last Modified: Wed, 01 Sep 2021 00:33:57 GMT  
		Size: 209.7 MB (209652643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
