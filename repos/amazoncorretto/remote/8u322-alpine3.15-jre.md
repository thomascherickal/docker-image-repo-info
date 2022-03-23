## `amazoncorretto:8u322-alpine3.15-jre`

```console
$ docker pull amazoncorretto@sha256:eadfa6670bfeaa74d6b20bda54dd3b2c558a533b045787e4167dc1a1a5facfc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u322-alpine3.15-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:db990123c873b3688f1975f630540fc2d64d506f14ac73d720590cf445643c26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43193770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93b5f234f57f53935ebd690ee7980274ae03672213ec73d8b4842a19d9c527dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 15:46:36 GMT
ARG version=8.322.06.2
# Wed, 23 Mar 2022 15:46:48 GMT
# ARGS: version=8.322.06.2
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 23 Mar 2022 15:46:48 GMT
ENV LANG=C.UTF-8
# Wed, 23 Mar 2022 15:46:48 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2eb574382a596c978d389c9a319270cac6e6f08aefa13866f1a18f5119540bc`  
		Last Modified: Wed, 23 Mar 2022 15:49:32 GMT  
		Size: 40.4 MB (40381081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
