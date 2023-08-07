## `amazoncorretto:11-alpine3.15`

```console
$ docker pull amazoncorretto@sha256:d7c5a60845c9275feddf42d2113f09eb8112ad65b6588d0d060ea11a40c58be5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-alpine3.15` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:03ba95895e10f47dfdc0d86f605ca3bbd1b93a4c40abeb669c307ac1ab4d46dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.2 MB (144204173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3adba90cfc53d48d97af095b7b44b36688a09c6fb017913fdb71232182c7afae`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:46:09 GMT
ARG version=11.0.20.8.1
# Mon, 07 Aug 2023 19:46:16 GMT
# ARGS: version=11.0.20.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0 &&     rm -rf /usr/lib/jvm/java-11-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 19:46:17 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 19:46:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 19:46:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84d62cb4583d6c653e3776d19cf3d22a690d0218e16ddd5b408484638ff814f`  
		Last Modified: Mon, 07 Aug 2023 19:53:00 GMT  
		Size: 141.4 MB (141378167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:1c3d9c185eab533b079d5c5a6f072c32eec67c6a7086c17bcf8edce769b380a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.4 MB (142370436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:753384a234d36357d8da90f7b2414e77e1c7d5681cc8182bed90ab78030a932f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:26:13 GMT
ARG version=11.0.20.8.1
# Mon, 07 Aug 2023 20:26:19 GMT
# ARGS: version=11.0.20.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0 &&     rm -rf /usr/lib/jvm/java-11-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 20:26:20 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:26:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 20:26:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03db325880ec1705f2573e151859de568d49f7329cf50823ff12669718dbcbd5`  
		Last Modified: Mon, 07 Aug 2023 20:39:25 GMT  
		Size: 139.6 MB (139649568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
