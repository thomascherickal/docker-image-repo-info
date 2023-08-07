## `amazoncorretto:20-alpine3.15`

```console
$ docker pull amazoncorretto@sha256:51097c9f4914b4deb203ea46961184399ca7f7da37f1adc34c24500184c1f559
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:20-alpine3.15` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:0c715ae0d924f24c8232c531f1a4e6650e074ca73492642cca9545bf67f2c70f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.4 MB (157400835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:999c03a2cd5708630c63b5224f3bd30e90edbdc4468d0cbb363ab50fad8abcc5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:47:43 GMT
ARG version=20.0.2.9.1
# Mon, 07 Aug 2023 19:47:49 GMT
# ARGS: version=20.0.2.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0 &&     rm -rf /usr/lib/jvm/java-20-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 19:47:49 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 19:47:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 19:47:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34243a12733d6eab003ff6342c910fc3f2465c8dcbac4147a7f8a8a4a8163ca0`  
		Last Modified: Mon, 07 Aug 2023 19:56:56 GMT  
		Size: 154.6 MB (154574829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:20-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:65cf4ad89385d29e55fb78dd76d2312d975142c5cb0381339cd94591cf3940f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155382247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9fc9da3235b0f66dad06f92ed97b9fa6d4dbed31aef0b49f2403171a1adba17`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:31:07 GMT
ARG version=20.0.2.9.1
# Mon, 07 Aug 2023 20:31:12 GMT
# ARGS: version=20.0.2.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-20=$version-r0 &&     rm -rf /usr/lib/jvm/java-20-amazon-corretto/lib/src.zip
# Mon, 07 Aug 2023 20:31:14 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:31:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 07 Aug 2023 20:31:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f893d00ead8f1f8d35f2660c0c321bd7ad7c5b1327fb085f2eacae9c0bf57d`  
		Last Modified: Mon, 07 Aug 2023 20:46:32 GMT  
		Size: 152.7 MB (152661379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
