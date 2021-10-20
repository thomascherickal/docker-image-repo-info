## `amazoncorretto:11-alpine3.14`

```console
$ docker pull amazoncorretto@sha256:e94eea4b57a71b7e33933a9f5ea5a8f23f433b920db8ff455d5d1a754eea7581
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine3.14` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:8a93f7bc0d8f5c30062b1fc27a72bba0c0f674a56716920dd4afaffea7a7493c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.1 MB (196142703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a26967833163e51cad0a5cac88084d55b9af8198a00152a0e4e1d84552b882a6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 20 Oct 2021 18:21:19 GMT
ARG version=11.0.13.8.1
# Wed, 20 Oct 2021 18:21:25 GMT
# ARGS: version=11.0.13.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Wed, 20 Oct 2021 18:21:26 GMT
ENV LANG=C.UTF-8
# Wed, 20 Oct 2021 18:21:26 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Wed, 20 Oct 2021 18:21:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1e30640b5fa4a267092430cd69a6d5c8a91ebadc1b89be97ee8cdd2b9cb8d7`  
		Last Modified: Wed, 20 Oct 2021 18:27:36 GMT  
		Size: 193.3 MB (193328257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
