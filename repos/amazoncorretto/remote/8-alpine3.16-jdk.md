## `amazoncorretto:8-alpine3.16-jdk`

```console
$ docker pull amazoncorretto@sha256:1f7623d7e53db5e651d88ae87ce2a70a2feb03d43d0e48e2783ef87d5341cd61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-alpine3.16-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:289ed664e038492294b673e70636eb0ebf09d9d14bbef3f11a1c6df376d3fb4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102864826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac7310291fd5d4bce26c763311739f5ec602dc8e468b47a16c4a2cf712e6efc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:45:13 GMT
ARG version=8.382.05.1
# Mon, 07 Aug 2023 19:45:17 GMT
# ARGS: version=8.382.05.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 19:45:17 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 19:45:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 19:45:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae95cb0b79a6a2be863336f5c83a3d3e7935ef405a0f71be44ac9c5360c860e9`  
		Last Modified: Mon, 07 Aug 2023 19:50:44 GMT  
		Size: 100.1 MB (100057143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-alpine3.16-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:ea6b4bd07363d18814dd86818863ab32d824fcdadeeeb15a764f1018791f08ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102499748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c58fe8bdaa9a233546bb28b082e1f59407f908fb6a49804186ba7e8394ca78bc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:23:07 GMT
ARG version=8.382.05.1
# Mon, 07 Aug 2023 20:23:11 GMT
# ARGS: version=8.382.05.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 20:23:12 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:23:13 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 20:23:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c4570cfc8344b3b4f7d261201a49a663dcc9e1c01c29e19f7a4ae7f52e818f`  
		Last Modified: Mon, 07 Aug 2023 20:35:14 GMT  
		Size: 99.8 MB (99791725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
