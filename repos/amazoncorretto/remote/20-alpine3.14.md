## `amazoncorretto:20-alpine3.14`

```console
$ docker pull amazoncorretto@sha256:304126c2f3a8451d5a3f3d9c14baa3db6c9a69940fcee0537feadcf80645741b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-alpine3.14` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d3346cddfee261c2dafad300bff858a72879ff80affa95ddcfaa3533518c7ddd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.6 MB (206557425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14f61e8fd66848b1fe10735829532c1c89f99cea200c7fdcd591b0e0c234713`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:19:50 GMT
ARG version=20.0.0.36.1
# Wed, 29 Mar 2023 19:19:56 GMT
# ARGS: version=20.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0
# Wed, 29 Mar 2023 19:19:56 GMT
ENV LANG=C.UTF-8
# Wed, 29 Mar 2023 19:19:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 29 Mar 2023 19:19:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f9b5424aab6dc13b07b660400159c31f0793d8b89b2e7645daf52a8297ab66`  
		Last Modified: Wed, 29 Mar 2023 19:29:44 GMT  
		Size: 203.7 MB (203727778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:4db3d647af4e3af8b6789e028acbd380bf5657e75bb9fd52420ed487d5ef5fbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.5 MB (204457084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e41cf4e417298b84f25755dffda8cbc7dc36f5619387e395ce74c0de8091b182`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:25 GMT
ADD file:c3d52cc254959a9ff493e7347e6b1bc25c0ccfdcf9532dbf43173ddd182d0e4d in / 
# Wed, 29 Mar 2023 17:39:25 GMT
CMD ["/bin/sh"]
# Thu, 20 Apr 2023 17:45:05 GMT
ARG version=20.0.1.9.1
# Thu, 20 Apr 2023 17:45:13 GMT
# ARGS: version=20.0.1.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0
# Thu, 20 Apr 2023 17:45:15 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:45:15 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 20 Apr 2023 17:45:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:422ed46b1a92579f7c475c0c19fade6880a8d98f23a2b4ccfb77c265d4f72dfc`  
		Last Modified: Wed, 29 Mar 2023 17:40:13 GMT  
		Size: 2.7 MB (2725148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7033c6a501e8145fccfa61fa75296d537a9098ce1cba7dcc70d611b247c89069`  
		Last Modified: Thu, 20 Apr 2023 17:56:42 GMT  
		Size: 201.7 MB (201731936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
