## `amazoncorretto:17-alpine3.13-jdk`

```console
$ docker pull amazoncorretto@sha256:0f95b13288efb308c0c70199ef9cce9f94fc6f72abe4296cb7baa708eb59dff2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.13-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:8c0691a9ded6d1f8f6c0d12b69482a8fdb534078f376d1515b6b3ff3c13aa146
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194484358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a14f31e14499d053a73e734b9bab24ff079126f0a418a04a9745292c4861c08`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:14 GMT
ADD file:7fd90c097e2c4587dee91726d71abc02fa1aa6a3a3395c862206a4e14e0c299c in / 
# Tue, 09 Aug 2022 17:20:14 GMT
CMD ["/bin/sh"]
# Tue, 16 Aug 2022 23:21:16 GMT
ARG version=17.0.4.9.1
# Tue, 16 Aug 2022 23:21:22 GMT
# ARGS: version=17.0.4.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Tue, 16 Aug 2022 23:21:23 GMT
ENV LANG=C.UTF-8
# Tue, 16 Aug 2022 23:21:23 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 16 Aug 2022 23:21:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:72cfd02ff4d01b1f319eed108b53120dea0185b916d2abeb4e6121879cbf7a65`  
		Last Modified: Tue, 09 Aug 2022 17:21:16 GMT  
		Size: 2.8 MB (2827571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43db261755afd098ff7d5c9403b46b66df31f0b9fdbfdbb2381764fff13da93`  
		Last Modified: Tue, 16 Aug 2022 23:26:17 GMT  
		Size: 191.7 MB (191656787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
