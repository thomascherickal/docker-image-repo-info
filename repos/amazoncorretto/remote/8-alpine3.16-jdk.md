## `amazoncorretto:8-alpine3.16-jdk`

```console
$ docker pull amazoncorretto@sha256:33bc2ca0e588e58de2de328f30e958d8d6ab270e0799499ae0e9a765bbbc3b29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-alpine3.16-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:00e7e7516a9d341b618fdaf210330daf34fac5eed40eb75e2784f71972339d51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102868874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425024e3a2e970d8229179dca31a6651447a01ebb352cbdd5e7be8e4a67f06a2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Thu, 19 Oct 2023 03:17:28 GMT
ARG version=8.392.08.1
# Thu, 19 Oct 2023 03:17:32 GMT
# ARGS: version=8.392.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Thu, 19 Oct 2023 03:17:33 GMT
ENV LANG=C.UTF-8
# Thu, 19 Oct 2023 03:17:33 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 19 Oct 2023 03:17:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c54412c4da260b3a4beef920c7d1da05fe3010d32868a07bb203c491903095`  
		Last Modified: Thu, 19 Oct 2023 03:33:36 GMT  
		Size: 100.1 MB (100061191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-alpine3.16-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d4d383b46b84fc3ef64e3b85a76a6577ce9311eb809cce6272d4e3cfa2b39915
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102514199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08efa175032ab2302a95ebf01b483e3dd35fadbe987a28bca7c70acf143566db`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:11 GMT
ADD file:1efd26ad638f3c262f37eb81a32e3f026121dcd60479e91c42097bfc8329ed3b in / 
# Thu, 30 Nov 2023 23:11:11 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:44:32 GMT
ARG version=8.392.08.1
# Fri, 01 Dec 2023 02:44:37 GMT
# ARGS: version=8.392.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0 &&     rm -rf /usr/lib/jvm/java-8-amazon-corretto/lib/src.zip
# Fri, 01 Dec 2023 02:44:39 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 02:44:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 01 Dec 2023 02:44:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:5362b5901f8a9898f2bcc8eb6c3e6990364aa058617afaae388bdb9f437d3d7e`  
		Last Modified: Thu, 30 Nov 2023 23:11:54 GMT  
		Size: 2.7 MB (2708293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf26f8c36c64d83253a6f093b03f529b7f67720492566540d317d42099c93fab`  
		Last Modified: Fri, 01 Dec 2023 02:48:34 GMT  
		Size: 99.8 MB (99805906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
