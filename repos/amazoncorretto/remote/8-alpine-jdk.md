## `amazoncorretto:8-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:1b949d30bf0cb61cbdf64bc942f755033eec87add138d083cd38d114c3ccebfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6eff7dbac1dd7a891aa0c5986e05843dbd7abd7bf2630a3500a04902667b49ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101612075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08399a8f4d143f44b2190d7e21740b766691148fe319209a20da222eb26fc81b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Fri, 29 Jul 2022 20:20:26 GMT
ARG version=8.342.07.4
# Fri, 29 Jul 2022 20:20:30 GMT
# ARGS: version=8.342.07.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Fri, 29 Jul 2022 20:20:31 GMT
ENV LANG=C.UTF-8
# Fri, 29 Jul 2022 20:20:31 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 29 Jul 2022 20:20:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45f4017e9da6646a36c4cdc8d62ad21417f30d38cb567b06c37607e5985d676`  
		Last Modified: Fri, 29 Jul 2022 20:24:21 GMT  
		Size: 98.8 MB (98797430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
