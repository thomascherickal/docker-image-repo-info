## `amazoncorretto:11-alpine3.15-full`

```console
$ docker pull amazoncorretto@sha256:8521f977f5d51118ada5e1624f72a19013c5e96fea3967abb1402bf7e6dafc2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine3.15-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3ebb3eae1a03ddbfd7354ef60f8f8a4dabbca490e00814784f818a1884992bb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196276132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e8ea263115c8ee6aed3c018708d1d7c957c737ada1d6e25d68923bf2c609706`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 15:46:59 GMT
ARG version=11.0.14.9.1
# Wed, 23 Mar 2022 15:47:07 GMT
# ARGS: version=11.0.14.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 23 Mar 2022 15:47:08 GMT
ENV LANG=C.UTF-8
# Wed, 23 Mar 2022 15:47:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 23 Mar 2022 15:47:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b7a9e3ca13e6d625e2c6ed6a3aebf72d3f41c4ea50c1b94b2ca4aea6f378a9`  
		Last Modified: Wed, 23 Mar 2022 15:50:07 GMT  
		Size: 193.5 MB (193463443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
