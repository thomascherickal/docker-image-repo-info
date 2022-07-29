## `amazoncorretto:8u342-alpine-jre`

```console
$ docker pull amazoncorretto@sha256:f42713d0630c1891b19e0baf8c21449e2e998ccfd6a275be8f4a7f886dcfa6c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u342-alpine-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6e35e08b265a8988045835ee790a6eebc2231aa3f31278ce28a0e7107c19b615
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43254205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7c0ea1db676c47a9830c0d2cc8537f8c0b8fa67f133b4926f23514b79666f4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Fri, 29 Jul 2022 20:20:26 GMT
ARG version=8.342.07.4
# Fri, 29 Jul 2022 20:20:37 GMT
# ARGS: version=8.342.07.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Fri, 29 Jul 2022 20:20:37 GMT
ENV LANG=C.UTF-8
# Fri, 29 Jul 2022 20:20:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a7d643aca3273e98bc95ed2f33171d32468800b5dc93a6f1b535c6237c1e83`  
		Last Modified: Fri, 29 Jul 2022 20:24:52 GMT  
		Size: 40.4 MB (40439560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
