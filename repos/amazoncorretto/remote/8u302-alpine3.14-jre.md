## `amazoncorretto:8u302-alpine3.14-jre`

```console
$ docker pull amazoncorretto@sha256:0cc45b6b97ef3954754ce68c9066c2b453aa6d3b22cc5b3916199f05ea3b1537
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u302-alpine3.14-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:a7c4f8c4f51f8cc33614873c823ef0b5b97387fcf5d1badb8b52247a7ca90f81
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43163273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be263125ac59c09529eee2096dbfa7273c81aaf27889f0ddebdc55a805ae41e7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 02 Oct 2021 01:19:53 GMT
ARG version=8.302.08.1
# Sat, 02 Oct 2021 01:20:04 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Sat, 02 Oct 2021 01:20:04 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 01:20:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95721ef482300e43feef5961fc4e393891f7514268146aed2c9183bee97c5eb`  
		Last Modified: Tue, 05 Oct 2021 17:23:21 GMT  
		Size: 40.3 MB (40348827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
