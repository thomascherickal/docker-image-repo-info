## `amazoncorretto:8u312-alpine3.13-jre`

```console
$ docker pull amazoncorretto@sha256:685f4e0c07879fa4cbcb9d86a88cada6e2c585840126941e707feafd5ab81496
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u312-alpine3.13-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:50117762b1e29df1727ce8d08969c79043aaae76e2ea0e398f631b6dbae36959
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43165607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d72b5745cc4f42eb3a75c10d2795beb25603620d1656e5a1a8de738cc7fbbe10`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 20 Oct 2021 18:20:06 GMT
ARG version=8.312.07.1
# Wed, 20 Oct 2021 18:20:16 GMT
# ARGS: version=8.312.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 20 Oct 2021 18:20:16 GMT
ENV LANG=C.UTF-8
# Wed, 20 Oct 2021 18:20:16 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9998f71681e8a588879f8ed37af3b2a1df1ad0844575528eb0deed6d14558`  
		Last Modified: Wed, 20 Oct 2021 18:24:59 GMT  
		Size: 40.4 MB (40351528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
