## `amazoncorretto:8u372-alpine3.17-jre`

```console
$ docker pull amazoncorretto@sha256:e25c78667ef2874dd3ec84fba3c6136562e7e53bf06cc995787cbeb565288ca8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u372-alpine3.17-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5776a044676a8e16f25accbc525b27f8df79b986e5d9bf64d691078f46c30865
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44894173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af5ae74e69dfc92c468631653f8d22e3d2b5e478d5b00ff3babed7dcd3a1785`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:34:45 GMT
ARG version=8.372.07.1
# Thu, 15 Jun 2023 05:34:55 GMT
# ARGS: version=8.372.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Thu, 15 Jun 2023 05:34:56 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 05:34:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e808d00ccc4eb4bc68d53565f37f88e156d525ac1089c237007bd5bcab8b15`  
		Last Modified: Thu, 15 Jun 2023 05:39:39 GMT  
		Size: 41.5 MB (41519460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u372-alpine3.17-jre` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:fba2b81d1eb056228ed120b5e680274a1d89735c20876d5c089883643b351c30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44526783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e41fc231d9a670462a5858c377be63cd7b0b5214ca19a3c2b823fec8673de8d2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:08:08 GMT
ARG version=8.372.07.1
# Wed, 14 Jun 2023 22:08:16 GMT
# ARGS: version=8.372.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 14 Jun 2023 22:08:16 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jun 2023 22:08:16 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b883b6f26374bcd460ab23bd76cc215f879be6ccc3a158d8f861a86b3502a552`  
		Last Modified: Wed, 14 Jun 2023 22:12:43 GMT  
		Size: 41.3 MB (41265644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
