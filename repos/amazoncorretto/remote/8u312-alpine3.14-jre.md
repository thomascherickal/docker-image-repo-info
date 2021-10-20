## `amazoncorretto:8u312-alpine3.14-jre`

```console
$ docker pull amazoncorretto@sha256:63aa136ff25ad42763e930740ea76c1e728fed07c00405aac916c7da1523b7ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u312-alpine3.14-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:cab6ecbb4cd8b085b23f35c64cab169b5a38d9afd8e3955f457ae06ff058fdf4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43174294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bf1e1f0b3a8a2a73faff62b354fe9fcc7563ed1756d1b50106e5567dc1cc362`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 20 Oct 2021 18:20:19 GMT
ARG version=8.312.07.1
# Wed, 20 Oct 2021 18:20:29 GMT
# ARGS: version=8.312.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 20 Oct 2021 18:20:29 GMT
ENV LANG=C.UTF-8
# Wed, 20 Oct 2021 18:20:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550cacece9dec1c6269c1d8d0bd7a4d71eae3af23b95ad7c28a09f83e1d42eb3`  
		Last Modified: Wed, 20 Oct 2021 18:25:35 GMT  
		Size: 40.4 MB (40359848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
