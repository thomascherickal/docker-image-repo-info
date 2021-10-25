## `amazoncorretto:17-alpine3.14-full`

```console
$ docker pull amazoncorretto@sha256:782fb406f222a96d98a85ba7ed6d50483ff405a94a79823aa6903f91177e9b21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.14-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:7b1d95a3fc751fe0ea78eb6f2a88399fba9495c3793476286982057fae5e43fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194580713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e18f22d09ada8a640f4a077784194ae09565572db7437467e0c6b5f729b9d96`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Mon, 25 Oct 2021 18:24:51 GMT
ARG version=17.0.1.12.1
# Mon, 25 Oct 2021 18:24:57 GMT
# ARGS: version=17.0.1.12.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Mon, 25 Oct 2021 18:24:58 GMT
ENV LANG=C.UTF-8
# Mon, 25 Oct 2021 18:24:58 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 25 Oct 2021 18:24:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00133422db76c4ab20b351c7ef0922110c0685e4cc8571afd6aa998cbba1408b`  
		Last Modified: Mon, 25 Oct 2021 18:28:33 GMT  
		Size: 191.8 MB (191766267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
