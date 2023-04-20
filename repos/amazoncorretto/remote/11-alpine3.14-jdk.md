## `amazoncorretto:11-alpine3.14-jdk`

```console
$ docker pull amazoncorretto@sha256:0dec1c6bc68b59253c065410afda8f9b9d9e4cc448dfaaaf35ef7a28042439c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-alpine3.14-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:101d71c8a6254d8e8b03df90e039dd8ab1f5ae1d5fa1050190246030b2d6b076
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (197963009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b17c2bd5380c3e416694e97cfc58a6e54e6e98e19192248f07cdf0e81eb203`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:37 GMT
ADD file:9663235f252e072c52b0f9e25845841e4321cce2caa7467a0d736c6003b05c00 in / 
# Wed, 29 Mar 2023 18:19:37 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:17:58 GMT
ARG version=11.0.18.10.1
# Wed, 29 Mar 2023 19:18:04 GMT
# ARGS: version=11.0.18.10.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 29 Mar 2023 19:18:04 GMT
ENV LANG=C.UTF-8
# Wed, 29 Mar 2023 19:18:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 29 Mar 2023 19:18:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:f7dab3ab2d6ec29aa28769bec35331fb485b5837501b1e8556413d8b5a79c9c8`  
		Last Modified: Wed, 29 Mar 2023 18:20:25 GMT  
		Size: 2.8 MB (2829647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fca3dcd726ba5d688c094ae0a9a65fdcbf878c305311884d3290ccb07b6c10`  
		Last Modified: Wed, 29 Mar 2023 19:24:06 GMT  
		Size: 195.1 MB (195133362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-alpine3.14-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:edb77897d7a385d971b50ea9f83fdf5ab7aa78d44c2bb3956350d5e45dda0dac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.2 MB (196193964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b8745399177715eaedf9b575aac177d4a06d86433eda0c11fe593580f3abce4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:25 GMT
ADD file:c3d52cc254959a9ff493e7347e6b1bc25c0ccfdcf9532dbf43173ddd182d0e4d in / 
# Wed, 29 Mar 2023 17:39:25 GMT
CMD ["/bin/sh"]
# Thu, 20 Apr 2023 17:42:08 GMT
ARG version=11.0.19.7.1
# Thu, 20 Apr 2023 17:42:13 GMT
# ARGS: version=11.0.19.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Thu, 20 Apr 2023 17:42:15 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:42:15 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 20 Apr 2023 17:42:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:422ed46b1a92579f7c475c0c19fade6880a8d98f23a2b4ccfb77c265d4f72dfc`  
		Last Modified: Wed, 29 Mar 2023 17:40:13 GMT  
		Size: 2.7 MB (2725148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a420344064c8d1ba1004841ccd73768db44fc587864acfabc662a5d44435eb82`  
		Last Modified: Thu, 20 Apr 2023 17:51:28 GMT  
		Size: 193.5 MB (193468816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
