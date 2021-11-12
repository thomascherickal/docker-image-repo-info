## `amazoncorretto:11-alpine3.12-jdk`

```console
$ docker pull amazoncorretto@sha256:ef2886b495fe8f7ed7178a7b1f4484aa8fe713e1db81e13442a077a4a97692f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine3.12-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b8b0d131104b052c1350e7b1390cf52c223e46413b4c3dd16c1fc828748578da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196133326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fb79418920cc671fca2b56455ef460f0ebfd82206e8f50b9755e2c8418b6a36`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:19:14 GMT
ARG version=11.0.13.8.1
# Fri, 12 Nov 2021 21:19:20 GMT
# ARGS: version=11.0.13.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Fri, 12 Nov 2021 21:19:20 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:19:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 12 Nov 2021 21:19:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63eb5b7f205e5806804c13fc43c7950467a1e8c58a5b044e24bff5f5f613051`  
		Last Modified: Fri, 12 Nov 2021 21:25:11 GMT  
		Size: 193.3 MB (193323853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
