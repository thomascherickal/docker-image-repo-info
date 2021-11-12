## `amazoncorretto:8-alpine3.13-jdk`

```console
$ docker pull amazoncorretto@sha256:8ce47c3dcfa1768302a0252ccedea4e431430032df2e29bedfdf0b9a9ab79185
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.13-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:212d39e236a556fbc21b91f7580959c08bd6c3e39c613feaf1019878e975c7a6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101880995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3c1292fd83ad65da815827ddce47f53771daabab8b62a62df13b724dbbab19`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:18:43 GMT
ARG version=8.312.07.1
# Fri, 12 Nov 2021 21:18:48 GMT
# ARGS: version=8.312.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Fri, 12 Nov 2021 21:18:48 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:18:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 12 Nov 2021 21:18:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6504d29bf2c97cf58cbc26027a9fb8b94d1416f2a46ae9cb4e0c5e90659375ae`  
		Last Modified: Fri, 12 Nov 2021 21:23:32 GMT  
		Size: 99.1 MB (99058570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
