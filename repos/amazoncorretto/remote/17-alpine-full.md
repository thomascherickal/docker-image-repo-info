## `amazoncorretto:17-alpine-full`

```console
$ docker pull amazoncorretto@sha256:e42444c2fccfe699a568eaf3d3baa929a38d365ec561f459ecf5f0d529e26c67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c3445d61df8a764cf4f2645a2a9ab92cfe1ace5864e1210efebef3956db49b97
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.8 MB (194756538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:542966b432a459ee4c5a196c7fc566949a0499bcd5ea4b734779dae20e39a9d8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 22:25:56 GMT
ARG version=17.0.3.6.1
# Tue, 19 Apr 2022 22:26:01 GMT
# ARGS: version=17.0.3.6.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Tue, 19 Apr 2022 22:26:02 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:26:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Apr 2022 22:26:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77803fb10f7b755671b92b8de1246bda9f0847f496a92c6b6ff9b92b5e7533b3`  
		Last Modified: Tue, 19 Apr 2022 22:36:55 GMT  
		Size: 191.9 MB (191941979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
