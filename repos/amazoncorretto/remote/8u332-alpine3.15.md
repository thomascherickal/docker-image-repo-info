## `amazoncorretto:8u332-alpine3.15`

```console
$ docker pull amazoncorretto@sha256:ce02f69f8edbc477d236e38ed07791c13efa70e3f4d52cadfd6017ffc6177aab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u332-alpine3.15` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:69547483b36a0b3d1c223ad27e62e7b7ac91ee2fde135288eaad7b0bc3ef9e56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101778448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba06778d17ea4cea5c230a9a4bbc5adfb46e7db7068093dba60aeda3e6f33f10`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 22:23:33 GMT
ARG version=8.332.08.1
# Tue, 19 Apr 2022 22:23:37 GMT
# ARGS: version=8.332.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 19 Apr 2022 22:23:37 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:23:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Apr 2022 22:23:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb0666b0d84aa9c6b32339874dec9a70eae35ccc8268ea6f55a8aa90252e8e2`  
		Last Modified: Tue, 19 Apr 2022 22:31:32 GMT  
		Size: 99.0 MB (98963889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
