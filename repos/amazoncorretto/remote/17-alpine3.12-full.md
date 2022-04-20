## `amazoncorretto:17-alpine3.12-full`

```console
$ docker pull amazoncorretto@sha256:1ad3e68a9abe1c4811550463a1c4dfa16f6dd5f4330a526d0241cad58ee08d39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.12-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:8124ad3955c5876d8b0a55fa7cf227b4ec31b52009a9a3989d54febacd9737f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194737843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06d9570c1ce26589a1932f98374440feb592f38de904597d8994af74333d21ad`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:19 GMT
ADD file:c1aa87a3b464fca64d769444b5201bc0426a1f517c91c4a7916270e10f8b300b in / 
# Tue, 05 Apr 2022 00:20:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 22:25:20 GMT
ARG version=17.0.3.6.1
# Tue, 19 Apr 2022 22:25:34 GMT
# ARGS: version=17.0.3.6.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Tue, 19 Apr 2022 22:25:34 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:25:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Apr 2022 22:25:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:1b7ca6aea1ddfe716f3694edb811ab35114db9e93f3ce38d7dab6b4d9270cb0c`  
		Last Modified: Tue, 05 Apr 2022 00:21:10 GMT  
		Size: 2.8 MB (2808060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc06b970640047d7e7029e49c48e1393b2675189f379843fabc3d0348d1a0c7`  
		Last Modified: Tue, 19 Apr 2022 22:35:28 GMT  
		Size: 191.9 MB (191929783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
