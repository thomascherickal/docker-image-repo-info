## `amazoncorretto:8u302-alpine3.13`

```console
$ docker pull amazoncorretto@sha256:ed7d7cb1a866c0e1b02d852e2defaa26b14f66c211020b012f505fb3166b1573
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u302-alpine3.13` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6a92d4035584de7e88dd121dde2f3bb231b8f1913b6d8779cd5734a72c92024b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101845964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5993eaa1c831acdcc3f6325445177b4b393f7d034c5bd2659e5c612f26373990`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Sat, 02 Oct 2021 01:19:37 GMT
ARG version=8.302.08.1
# Sat, 02 Oct 2021 01:19:42 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Sat, 02 Oct 2021 01:19:43 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 01:19:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Sat, 02 Oct 2021 01:19:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aee78ec405883146d91facac3bf7956843f64762e6318f00f3e2020a2677a18`  
		Last Modified: Tue, 05 Oct 2021 17:22:25 GMT  
		Size: 99.0 MB (99031885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
