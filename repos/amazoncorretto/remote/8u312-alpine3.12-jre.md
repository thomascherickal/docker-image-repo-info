## `amazoncorretto:8u312-alpine3.12-jre`

```console
$ docker pull amazoncorretto@sha256:6af3feab5c001f0c3e23140d37d4ade855c1f810f34ef30e2d48c5ce1fa9f955
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u312-alpine3.12-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:744847233d3827f4be580194f231c509e4b1a4b394dae0cafe60f1c5b7e6f315
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43162003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772fcbb486c6fa5c47260361976dbcf0422601f4abb098ef9bf33732a93cd986`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:18:21 GMT
ARG version=8.312.07.1
# Fri, 12 Nov 2021 21:18:40 GMT
# ARGS: version=8.312.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Fri, 12 Nov 2021 21:18:40 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:18:40 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425ca4afad7dcd336b27471241e6f2a9bb46ce0aa9ef96ed0f08f0f4f2e397b`  
		Last Modified: Fri, 12 Nov 2021 21:23:06 GMT  
		Size: 40.4 MB (40352530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
