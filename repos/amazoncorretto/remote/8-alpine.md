## `amazoncorretto:8-alpine`

```console
$ docker pull amazoncorretto@sha256:be8ad0fbb94e6a77c58dc5c4dab511c9f0d6035295ae92030cec31dd444f2acc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:8-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:fa637da49fd1ee8d14cbca7964cea0a2ac5539dfb9d5f2cf1206357916332afd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101784071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:196ebd92880142956bc8afa43e6c4eb5e030629476cf4968d5036cacdcdebe49`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:28:57 GMT
ARG version=8.282.08.1
# Thu, 01 Apr 2021 13:29:01 GMT
# ARGS: version=8.282.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Thu, 01 Apr 2021 13:29:02 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 13:29:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 01 Apr 2021 13:29:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe55e116d73706ae7e7eac497fc50e47544c2059e83b7b74c9d5d93587758bd`  
		Last Modified: Thu, 01 Apr 2021 13:30:57 GMT  
		Size: 99.0 MB (98984359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
