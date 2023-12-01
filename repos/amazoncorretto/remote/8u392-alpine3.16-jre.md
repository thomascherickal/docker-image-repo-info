## `amazoncorretto:8u392-alpine3.16-jre`

```console
$ docker pull amazoncorretto@sha256:39109ff5089a28beef52e8f9f4a4bafcfcbf8a038d22d2c164dae4c2bd86e5ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u392-alpine3.16-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ef48e7efc6eb290dd75a643483b0f187292fb183a4bc2458822f7a1f68dce5ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44346245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008f06330c4331bdd23e79e0e3905963f0a7bca7c07c8a4718ed74412eda1686`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 03:17:28 GMT
ARG version=8.392.08.1
# Thu, 19 Oct 2023 03:17:38 GMT
# ARGS: version=8.392.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Thu, 19 Oct 2023 03:17:38 GMT
ENV LANG=C.UTF-8
# Thu, 19 Oct 2023 03:17:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd3a72e3b99997ca4b43b0745ab9b1a7d7c80a669b9e0791c6c5fe2340d14bd`  
		Last Modified: Thu, 19 Oct 2023 03:33:54 GMT  
		Size: 41.5 MB (41538562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u392-alpine3.16-jre` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e62dc9b3c8676bf9e6f04116a33cc8934c93d22d16233deadc3d19f24e245cfd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43997329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:881c85485ff7b08b44f3ef6b870bdc2902f7ec00f253702f8a27ad5b0d5758cc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:11 GMT
ADD file:1efd26ad638f3c262f37eb81a32e3f026121dcd60479e91c42097bfc8329ed3b in / 
# Thu, 30 Nov 2023 23:11:11 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:44:32 GMT
ARG version=8.392.08.1
# Fri, 01 Dec 2023 02:44:44 GMT
# ARGS: version=8.392.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Fri, 01 Dec 2023 02:44:45 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 02:44:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:5362b5901f8a9898f2bcc8eb6c3e6990364aa058617afaae388bdb9f437d3d7e`  
		Last Modified: Thu, 30 Nov 2023 23:11:54 GMT  
		Size: 2.7 MB (2708293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930f750906c03abd1a1e68933a56ef4dc4fade37139e90e63b68419e889e45f1`  
		Last Modified: Fri, 01 Dec 2023 02:48:50 GMT  
		Size: 41.3 MB (41289036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
