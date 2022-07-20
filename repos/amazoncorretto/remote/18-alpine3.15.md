## `amazoncorretto:18-alpine3.15`

```console
$ docker pull amazoncorretto@sha256:1b1467a9ff0bf19f1b9718b9af69c1428b64bda76524286fbb33a30a8161fe09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:18-alpine3.15` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:da2ffeba6be71fb76f715a3566e4583b7956ceaf461925df9fcbb01cdd4e3a7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195675546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf3ba74a53a8715959b73cdade172e0c836447639532ad17478d58f715d5d60`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 22:40:20 GMT
ARG version=18.0.2.9.1
# Tue, 19 Jul 2022 22:40:26 GMT
# ARGS: version=18.0.2.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-18=$version-r0
# Tue, 19 Jul 2022 22:40:27 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:40:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Jul 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e2ce20b7961833ee0c60541a3ab07ac45afb43bae81af99763c9f3c039de6c`  
		Last Modified: Tue, 19 Jul 2022 22:50:07 GMT  
		Size: 192.9 MB (192860901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
