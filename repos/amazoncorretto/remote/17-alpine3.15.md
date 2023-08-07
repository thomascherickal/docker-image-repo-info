## `amazoncorretto:17-alpine3.15`

```console
$ docker pull amazoncorretto@sha256:fae7c1dd0cbc0d9139c8abceff8a3589f8b0be448a89777b21c0f98b5aebc858
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-alpine3.15` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:bb79b6170884c9cca5c89d17c41fcb82380baf3c7ec430386189b9bc4e80076d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.6 MB (148563953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9754b657f9344986061d4a859829a3c071b7bb3f9c02e2ee11085b6d49ef8b56`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:47:03 GMT
ARG version=17.0.8.7.1
# Mon, 07 Aug 2023 19:47:09 GMT
# ARGS: version=17.0.8.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0 &&     rm -rf /usr/lib/jvm/java-17-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 19:47:09 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 19:47:09 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 19:47:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cc639409543278631991c19cda4f592efc35948c977e93f8862ffbef5cd677`  
		Last Modified: Mon, 07 Aug 2023 19:55:00 GMT  
		Size: 145.7 MB (145737947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:556d526a70594612179ba3ee25947df5cc0923735899175868b496cfece06464
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.9 MB (146856769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15d3137f5d81f33b7084acaf0f5780efaff1d5987705f19e28a4852d5b0a265`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:29:41 GMT
ARG version=17.0.8.7.1
# Mon, 07 Aug 2023 20:29:47 GMT
# ARGS: version=17.0.8.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0 &&     rm -rf /usr/lib/jvm/java-17-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 20:29:49 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:29:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 20:29:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42e84cebb820808dc17ac603b3dc6655d499b7cb9f306d2a596a5511a0bb614`  
		Last Modified: Mon, 07 Aug 2023 20:43:44 GMT  
		Size: 144.1 MB (144135901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
