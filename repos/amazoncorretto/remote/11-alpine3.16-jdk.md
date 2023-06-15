## `amazoncorretto:11-alpine3.16-jdk`

```console
$ docker pull amazoncorretto@sha256:89e0f9bd21ab651341f30b9e76f6a6deb1d6de1c5b5d866a776806af65731f22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-alpine3.16-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b7ce6f24089f1d70bc69d7e0446352e4a7401b413fb4a64562130064d8f372fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197990163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c7d3b20ce0e55ccd47afd00f859cb68d6107072ad45d7e10f65fd2becfd5f2f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:35:23 GMT
ARG version=11.0.19.7.1
# Thu, 15 Jun 2023 05:35:29 GMT
# ARGS: version=11.0.19.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Thu, 15 Jun 2023 05:35:29 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 05:35:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 15 Jun 2023 05:35:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4f93b7b498a066cdd0e943a687f7c721a4e3e8565beadb3e34e6644b8235f4`  
		Last Modified: Thu, 15 Jun 2023 05:40:33 GMT  
		Size: 195.2 MB (195182494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-alpine3.16-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:dbc48ed20b33c427614349fc60edecbfc9c51f4ede06c68ab73337a5f2ea1de3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196176550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce7f4c7757ea0ce658447a0efac8f4919cc35cdf38cf015d3caf3ee736909ddc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:08:36 GMT
ARG version=11.0.19.7.1
# Wed, 14 Jun 2023 22:08:41 GMT
# ARGS: version=11.0.19.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 14 Jun 2023 22:08:43 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jun 2023 22:08:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 14 Jun 2023 22:08:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8138d47bbe2cc07241b246d2a89576799c404b26a5e415c2ccef84946fa9df5`  
		Last Modified: Wed, 14 Jun 2023 22:13:34 GMT  
		Size: 193.5 MB (193468644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
