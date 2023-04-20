## `amazoncorretto:8u372-alpine3.15-jre`

```console
$ docker pull amazoncorretto@sha256:c5fb522d1638de8fd287eaabeb684cc0997282c7c80628f4e8a1069b3b7405c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `amazoncorretto:8u372-alpine3.15-jre` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:b70f08536ea11e2d0e960a19debf49d103f547752c77c048b52be29961a68684
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43987173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b659d3b3454e9ab97c5ac4f940cd9153dc6a6b274d8d7479c687839f51190c7e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 20 Apr 2023 17:40:13 GMT
ARG version=8.372.07.1
# Thu, 20 Apr 2023 17:40:22 GMT
# ARGS: version=8.372.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Thu, 20 Apr 2023 17:40:22 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:40:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57119b2bda94f81eafba0b18efb0f25cc8b8055f10f9150bcb5f44d0618bb0d2`  
		Last Modified: Thu, 20 Apr 2023 17:48:33 GMT  
		Size: 41.3 MB (41265171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
