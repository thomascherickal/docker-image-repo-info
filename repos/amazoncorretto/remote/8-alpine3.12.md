## `amazoncorretto:8-alpine3.12`

```console
$ docker pull amazoncorretto@sha256:fda6f236a6dffd2094ff73c84bdaa213945ee68b65880f66a56bafef03544609
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.12` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d0608258d11d0a016345725d8538cbd9e4ab75da11055b3e3f37dcfd517829fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101868185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fd0c8a14aad357a3066271e13bd898d60920aefa8a7fd4d2b6b9d846fa16b2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:18:21 GMT
ARG version=8.312.07.1
# Fri, 12 Nov 2021 21:18:31 GMT
# ARGS: version=8.312.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Fri, 12 Nov 2021 21:18:31 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:18:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 12 Nov 2021 21:18:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ca4917cdf2784f3e4580f4228c9629c8b930059bfcb1bbf97089761f357ac2`  
		Last Modified: Fri, 12 Nov 2021 21:22:36 GMT  
		Size: 99.1 MB (99058712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
