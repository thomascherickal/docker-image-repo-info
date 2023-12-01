## `amazoncorretto:17-alpine3.16-jdk`

```console
$ docker pull amazoncorretto@sha256:d693f17788a451d938ae6f1075a2c8b78b5b53ba0e3232045f5a02ecab2bc5e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-alpine3.16-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7df9813f4d4b3b442faea5831ee1c861a7868f72164d3331d7b27790a3a408d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.4 MB (148410944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fec09103be0800c7839026ddd8ce178f6fafdda3ec477f712dcf1d8a02290d5a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 03:25:57 GMT
ARG version=17.0.9.8.1
# Thu, 19 Oct 2023 03:26:03 GMT
# ARGS: version=17.0.9.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0 &&     rm -rf /usr/lib/jvm/java-17-amazon-corretto/lib/src.zip
# Thu, 19 Oct 2023 03:26:04 GMT
ENV LANG=C.UTF-8
# Thu, 19 Oct 2023 03:26:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 19 Oct 2023 03:26:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c06686ff250e149172af224b85110103c9920588204f0e80e40fb0648f4d23`  
		Last Modified: Thu, 19 Oct 2023 03:42:55 GMT  
		Size: 145.6 MB (145603261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-alpine3.16-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:03d02bf6f962399494ec939195dd44829d4432d1abd505f5442363941df4a02a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146722376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:171ffcd2552bb0d0f907df04d457d258b8c6a48cb928bc164d2d418c376caefd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:11 GMT
ADD file:1efd26ad638f3c262f37eb81a32e3f026121dcd60479e91c42097bfc8329ed3b in / 
# Thu, 30 Nov 2023 23:11:11 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:46:10 GMT
ARG version=17.0.9.8.1
# Fri, 01 Dec 2023 02:46:16 GMT
# ARGS: version=17.0.9.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0 &&     rm -rf /usr/lib/jvm/java-17-amazon-corretto/lib/src.zip
# Fri, 01 Dec 2023 02:46:17 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 02:46:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 01 Dec 2023 02:46:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:5362b5901f8a9898f2bcc8eb6c3e6990364aa058617afaae388bdb9f437d3d7e`  
		Last Modified: Thu, 30 Nov 2023 23:11:54 GMT  
		Size: 2.7 MB (2708293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689e1541e905efec96b6a608a97d3a7a6bcfdf5d973a46037e2a27bf6841664b`  
		Last Modified: Fri, 01 Dec 2023 02:51:38 GMT  
		Size: 144.0 MB (144014083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
