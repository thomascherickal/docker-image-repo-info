## `amazoncorretto:17-alpine3.13-full`

```console
$ docker pull amazoncorretto@sha256:f1e61e659d054a497fede66c261de4c0adcc99575f09b3dec066772ef70e614e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.13-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7a3f34b54a272e87f7aa714d65d928c10c5bb67f44faefbd711a3a671324d22b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194582387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:380425b71f085d2a788ce54bc00ec1f4bd5d7818b0a90f5085b1b9fca87f1b0d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:20:02 GMT
ARG version=17.0.1.12.1
# Fri, 12 Nov 2021 21:20:13 GMT
# ARGS: version=17.0.1.12.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Fri, 12 Nov 2021 21:20:14 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:20:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 12 Nov 2021 21:20:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226742a24704da3fa6eed6733977ecd3eb222f633ff495de4a225eb903e9571b`  
		Last Modified: Fri, 12 Nov 2021 21:27:34 GMT  
		Size: 191.8 MB (191759962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
