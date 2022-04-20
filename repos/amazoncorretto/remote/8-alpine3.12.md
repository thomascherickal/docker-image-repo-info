## `amazoncorretto:8-alpine3.12`

```console
$ docker pull amazoncorretto@sha256:f3180ff6eb4e29fd3a60154229e671d920ff481242e1b96eef1def4f2a27264c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.12` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b625bad5f66a641bc732c39a929a68cd71c62c58188dc1a5e07342f4e0965708
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101769332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80022f4f3c4d620e511642a626c33bd4e75600e68c6cefd0a462a999ea3b1fa5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:19 GMT
ADD file:c1aa87a3b464fca64d769444b5201bc0426a1f517c91c4a7916270e10f8b300b in / 
# Tue, 05 Apr 2022 00:20:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 22:22:55 GMT
ARG version=8.332.08.1
# Tue, 19 Apr 2022 22:23:00 GMT
# ARGS: version=8.332.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 19 Apr 2022 22:23:01 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:23:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Apr 2022 22:23:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:1b7ca6aea1ddfe716f3694edb811ab35114db9e93f3ce38d7dab6b4d9270cb0c`  
		Last Modified: Tue, 05 Apr 2022 00:21:10 GMT  
		Size: 2.8 MB (2808060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005f1a1c1f01d55ee7c981202c2e556d4c85f732ce6cbd466b026cab16a1ae36`  
		Last Modified: Tue, 19 Apr 2022 22:29:41 GMT  
		Size: 99.0 MB (98961272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
