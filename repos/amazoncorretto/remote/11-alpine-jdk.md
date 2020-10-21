## `amazoncorretto:11-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:cc0e10f2ac81f075ec856a8fb76f2a4c3ee9cec2fac8d7e9eb0c5f78f1092389
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:32f5224ad546ece3e072a5f26a19ca00e8214729dc1acd22c48350a1f1ca5015
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.0 MB (195004369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb1c42decaa941649eab6d8498c424c2b8ee1e442aebc4baf046352b2334af3b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 21 Oct 2020 18:20:18 GMT
ARG version=11.0.9.11.1
# Wed, 21 Oct 2020 18:20:24 GMT
# ARGS: version=11.0.9.11.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 21 Oct 2020 18:20:24 GMT
ENV LANG=C.UTF-8
# Wed, 21 Oct 2020 18:20:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 21 Oct 2020 18:20:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f39190b6b563bade4a16c3cc1bbcc65f4af5a23386d1db4c60dd6235661dc58`  
		Last Modified: Wed, 21 Oct 2020 18:21:40 GMT  
		Size: 192.2 MB (192206828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
