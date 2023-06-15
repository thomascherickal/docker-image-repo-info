## `amazoncorretto:17-alpine3.15-jdk`

```console
$ docker pull amazoncorretto@sha256:6efa2940a1fe9d21ec754b907113b9e2335998ac94574a49f457077acdd3ecc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-alpine3.15-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f63af21867bbeb3bca7840df63b4d92494a5ac0580e89f2609ccb5209fbe9e56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196402241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36162be4f8d02d6121036ec6f8fbced027a373bfd74c5d572337250ec38e2ca9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:13 GMT
ADD file:4fa8e307f595ecff485113fb0ec6e2320979eaa6fb3eb467d2433771a6f016e6 in / 
# Wed, 14 Jun 2023 20:42:13 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:35:51 GMT
ARG version=17.0.7.7.1
# Thu, 15 Jun 2023 05:35:58 GMT
# ARGS: version=17.0.7.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Thu, 15 Jun 2023 05:35:58 GMT
ENV LANG=C.UTF-8
# Thu, 15 Jun 2023 05:35:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 15 Jun 2023 05:35:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:0cdfa0c98ed79707cd91c5dd7ebd282aa2b976d86a9e699d7fc188cdb6be390e`  
		Last Modified: Wed, 14 Jun 2023 20:42:58 GMT  
		Size: 2.8 MB (2825916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29748024221d890638346bbbc26f5a75bc14806a824645780681c45d1e9b8a5d`  
		Last Modified: Thu, 15 Jun 2023 05:41:36 GMT  
		Size: 193.6 MB (193576325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-alpine3.15-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:a326866e153b941127ebc38deee8381a4e1eee6c6e370805ae0176b330f48da2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194710265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba613a587cd360de52a3699a922a6a5a690ebaf476ee9166996c0c66e632889d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:10 GMT
ADD file:2b463f242cb7bf946452bb4781838348ecbe80da144fbab09f51d7e050dc68f3 in / 
# Wed, 14 Jun 2023 20:49:11 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:09:02 GMT
ARG version=17.0.7.7.1
# Wed, 14 Jun 2023 22:09:09 GMT
# ARGS: version=17.0.7.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Wed, 14 Jun 2023 22:09:11 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jun 2023 22:09:11 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 14 Jun 2023 22:09:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a147224bf413aeffbbfcdcb5104d35c647256a5c32083f4d8134f09a4e74ddeb`  
		Last Modified: Wed, 14 Jun 2023 20:49:52 GMT  
		Size: 2.7 MB (2720801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d92fb2d76f0c95a9e927888ac0cf3d8bc70f8553ddb94e5aa59bdcf18d99fa8`  
		Last Modified: Wed, 14 Jun 2023 22:14:32 GMT  
		Size: 192.0 MB (191989464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
