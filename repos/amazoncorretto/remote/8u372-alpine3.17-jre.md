## `amazoncorretto:8u372-alpine3.17-jre`

```console
$ docker pull amazoncorretto@sha256:cd79f35fbdf8599892a40ee7529d5bcae5a3accbc7344fdee65a6a23abdd96ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazoncorretto:8u372-alpine3.17-jre` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:2ba7606243567c0713e090d86f8a47a33b582bce7686661ba588ac6411181f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44527451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98658f4763a538773953d6553d6723b068768b1121e1b7b43f09dc0247fbd5d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 20 Apr 2023 17:40:34 GMT
ARG version=8.372.07.1
# Thu, 20 Apr 2023 17:40:43 GMT
# ARGS: version=8.372.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Thu, 20 Apr 2023 17:40:43 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:40:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9178dbef60bc999022840f8ef4363596baf77a792ec50c559cf383c195ff3b7`  
		Last Modified: Thu, 20 Apr 2023 17:49:47 GMT  
		Size: 41.3 MB (41265597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
