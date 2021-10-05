## `amazoncorretto:8u302-alpine3.14`

```console
$ docker pull amazoncorretto@sha256:cee1d74f564ec34abd216ac20a5761725b991294c7ba20f95c2be12f278e7f27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u302-alpine3.14` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:92d39ebf8acef9d3bd379d59972ef99d4f46c91c6acfcea0aabeff24b9b10feb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101849693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee7ebcd0f7706321cc92924d723d52b84b50127527c18faa5b9b03cd57394aa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 02 Oct 2021 01:19:53 GMT
ARG version=8.302.08.1
# Sat, 02 Oct 2021 01:19:57 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Sat, 02 Oct 2021 01:19:57 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 01:19:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Sat, 02 Oct 2021 01:19:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ee6534ee967d9f75629356164a637aee194c4544301534ecac369db190cde6`  
		Last Modified: Tue, 05 Oct 2021 17:23:02 GMT  
		Size: 99.0 MB (99035247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
