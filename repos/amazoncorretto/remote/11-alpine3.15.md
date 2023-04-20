## `amazoncorretto:11-alpine3.15`

```console
$ docker pull amazoncorretto@sha256:ab19c1c05673d79c00707e8a6ce07e9b4842a45c3590c93354b8132e95ff3348
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-alpine3.15` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6473b345b65c47d7ec4d13f67e114291bff6fe92e85292ef2da96351feb8ec30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197959953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f8e7dbfe2b9121785890c1db8cb2d59b0ffe88bbee60539cf25063402d3e925`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:18:07 GMT
ARG version=11.0.18.10.1
# Wed, 29 Mar 2023 19:18:12 GMT
# ARGS: version=11.0.18.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 29 Mar 2023 19:18:13 GMT
ENV LANG=C.UTF-8
# Wed, 29 Mar 2023 19:18:13 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 29 Mar 2023 19:18:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa1c7dee7c930d9d2d94dd2e8fc55989a415a72df582c1a467aaa82ce21c313`  
		Last Modified: Wed, 29 Mar 2023 19:24:32 GMT  
		Size: 195.1 MB (195133357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:74c84c1ea379d25ae83229f2467bdf0216728a4d5c19f413020ebae133083dea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196190801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c224eb15e791952141e803f7b23a7e2a5e6e9da1cafbc0aa0b7c74ab92363de`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 20 Apr 2023 17:42:18 GMT
ARG version=11.0.19.7.1
# Thu, 20 Apr 2023 17:42:23 GMT
# ARGS: version=11.0.19.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Thu, 20 Apr 2023 17:42:25 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:42:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 20 Apr 2023 17:42:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a35b5247f64b272198c17c0e39fbe8136e9dd64b9363bc05051ac3ecc35a77`  
		Last Modified: Thu, 20 Apr 2023 17:51:52 GMT  
		Size: 193.5 MB (193468799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
