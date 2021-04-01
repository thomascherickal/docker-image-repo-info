## `amazoncorretto:16-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:446994400e815b413a125026ad31ba95ff6b010cb2adf52364004c9a9a712c49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:16-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:04c2f7dc18d123c20644e782d96622b971c08a1e950769bd0158082c9f639edc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.4 MB (212400004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10275c1615dd8e41ed5ce2ae5927e85989b8dc6c6dde4ffae2b024b41b2f3631`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:29:44 GMT
ARG version=16.0.0.36.1
# Thu, 01 Apr 2021 13:29:55 GMT
# ARGS: version=16.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-16=$version-r0
# Thu, 01 Apr 2021 13:29:56 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 13:29:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 01 Apr 2021 13:29:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e651c1f0991a47d4cf4bc357f1441e53f3c15d243a6ae42902cbf8bfc1b88b`  
		Last Modified: Thu, 01 Apr 2021 13:33:02 GMT  
		Size: 209.6 MB (209600292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
