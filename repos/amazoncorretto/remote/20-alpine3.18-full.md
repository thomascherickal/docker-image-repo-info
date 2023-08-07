## `amazoncorretto:20-alpine3.18-full`

```console
$ docker pull amazoncorretto@sha256:7feacc36fa16a770131d42ee42e675cdb86641734d53300d00727ca247f97edb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-alpine3.18-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3497face6dc34eaf8bab061c2548962ffa4ac7869b663714dbcfe0526ee76930
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.0 MB (157976241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ff1f32c5a25265cd7c6587bbe96706b00b6929a1e8be52ca2e08204c1c245fe`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:48:13 GMT
ARG version=20.0.2.9.1
# Mon, 07 Aug 2023 19:48:18 GMT
# ARGS: version=20.0.2.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0 &&     rm -rf /usr/lib/jvm/java-20-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 19:48:19 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 19:48:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 19:48:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bb316279add30d2cb23733ce448e2b9ee1f3a3937394304c3db09a99dda530`  
		Last Modified: Mon, 07 Aug 2023 19:58:12 GMT  
		Size: 154.6 MB (154574628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-alpine3.18-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:3e3e0e7d6a00b812a8f6f68d26f8e1f956e33b87412313e059543ad04de89864
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (155992200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7563c8707b9031beb025ea2d8d133d6dd30eb0a000a3f44e4dfb3c4655c2c4c0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:31:34 GMT
ARG version=20.0.2.9.1
# Mon, 07 Aug 2023 20:31:39 GMT
# ARGS: version=20.0.2.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0 &&     rm -rf /usr/lib/jvm/java-20-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 20:31:41 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:31:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 20:31:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246b479d1260072161a6727ae51155a701e96857db06ca470f8df275a4ceb55f`  
		Last Modified: Mon, 07 Aug 2023 20:47:46 GMT  
		Size: 152.7 MB (152661433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
