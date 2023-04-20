## `amazoncorretto:8u372-alpine3.16-jre`

```console
$ docker pull amazoncorretto@sha256:6d6f05afc07695b53da0b9af1dc54dd5d0423a7d7b8e1e3574be404c2ebec4c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazoncorretto:8u372-alpine3.16-jre` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:59628bbb39a7cb08b0703c23434001794c2de386ff2d64c038c942e2137d383b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43974425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fb6ecd1305fb7ae7e1c85670ec68cd5a643eec03359e3302913fe459c353c2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 20 Apr 2023 17:40:24 GMT
ARG version=8.372.07.1
# Thu, 20 Apr 2023 17:40:32 GMT
# ARGS: version=8.372.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Thu, 20 Apr 2023 17:40:32 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:40:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516fc43b2887d278ee2159761d93f9011e148e163e6e93315c0d6abd3507a80d`  
		Last Modified: Thu, 20 Apr 2023 17:49:05 GMT  
		Size: 41.3 MB (41265081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
