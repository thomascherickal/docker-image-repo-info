## `amazoncorretto:8-alpine3.18-full`

```console
$ docker pull amazoncorretto@sha256:83fe34448f1dd3592650fa9ed78b55731dc1538488d7e8de722b3aa8d2c3411b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-alpine3.18-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:58251b6f61cfa3a6a034534bebe1c09ddf177fe734f54a5629519e22d2375bd1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.5 MB (103458764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19d4e4ea4aa8eea593ecf72dbd6db07127e57b2f52740e498948eee7957b6771`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:45:41 GMT
ARG version=8.382.05.1
# Mon, 07 Aug 2023 19:45:46 GMT
# ARGS: version=8.382.05.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 19:45:46 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 19:45:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 19:45:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471cfef86fecf0a60857969f58b6d51b05d6cb281bdc0c07528a2f1bfe22be2b`  
		Last Modified: Mon, 07 Aug 2023 19:51:56 GMT  
		Size: 100.1 MB (100057151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-alpine3.18-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:3abce2f36bdacd1a4aaf42422f5b3b956d5062ae46ba4683799ff5bf2e18c2ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103122430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d244f0921ac689a4e6c79c7a95038e9d11342dfeaa80c0f138c1ec3c9ab94ef4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:23:30 GMT
ARG version=8.382.05.1
# Mon, 07 Aug 2023 20:23:33 GMT
# ARGS: version=8.382.05.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 20:23:34 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:23:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 20:23:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4aef5b98eba053a10d8ac1cbf45391174c722df0c1d3f19db84a47253b3786`  
		Last Modified: Mon, 07 Aug 2023 20:36:24 GMT  
		Size: 99.8 MB (99791663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
