## `amazoncorretto:8-alpine3.13-jre`

```console
$ docker pull amazoncorretto@sha256:6fbbe603d09a696fbc868ae1c728223e5bb1aff4b90f9db789137eeb0db182b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.13-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:b7670c58b359b1a3a28d7bfd2323dae8e292a751669ce9ca8327a419e117f8c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43261735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21fada054249ff51bbf3685e34960c5678724c12cd8f94680165a7c28de112c8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:14 GMT
ADD file:7fd90c097e2c4587dee91726d71abc02fa1aa6a3a3395c862206a4e14e0c299c in / 
# Tue, 09 Aug 2022 17:20:14 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:36:46 GMT
ARG version=8.342.07.4
# Tue, 09 Aug 2022 17:36:57 GMT
# ARGS: version=8.342.07.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Tue, 09 Aug 2022 17:36:57 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 17:36:57 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:72cfd02ff4d01b1f319eed108b53120dea0185b916d2abeb4e6121879cbf7a65`  
		Last Modified: Tue, 09 Aug 2022 17:21:16 GMT  
		Size: 2.8 MB (2827571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db4a4227d868d85ab1d18ca3b464bc5002feebfbcc8cdc18defa64cd410d2ac`  
		Last Modified: Tue, 09 Aug 2022 17:41:05 GMT  
		Size: 40.4 MB (40434164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
