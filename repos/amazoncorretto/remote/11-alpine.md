## `amazoncorretto:11-alpine`

```console
$ docker pull amazoncorretto@sha256:b9d5e959586c21e4d2e5fc1e83eb1b2b5b1dfe9a991a499d26e83956d604264c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:11-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:dd7e8cb7ba5970b12d36568cbe66162d9c4cd44f8eff8a197be209422ca39234
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.1 MB (195086483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80e0d1ca1e0196adfa963a5c4fdcf548b5f5e8afd21039b542d338ef08ed9d18`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 21 Jan 2021 19:20:36 GMT
ARG version=11.0.10.9.1
# Thu, 21 Jan 2021 19:20:43 GMT
# ARGS: version=11.0.10.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Thu, 21 Jan 2021 19:20:43 GMT
ENV LANG=C.UTF-8
# Thu, 21 Jan 2021 19:20:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 21 Jan 2021 19:20:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c85d4dd6beb5e76ff7ecf4549e9588d8ae1d73ea6c1045e3b3a6530ff03062b`  
		Last Modified: Thu, 21 Jan 2021 19:23:20 GMT  
		Size: 192.3 MB (192287417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
