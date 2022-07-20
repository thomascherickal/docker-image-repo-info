## `amazoncorretto:8u342-alpine3.14-jre`

```console
$ docker pull amazoncorretto@sha256:8c83d1b8deee92b9f117b8cb3c639335c6e2d16dbb025960c317b277f7c406f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u342-alpine3.14-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:73b2b5a8b7fffd2b5524dcdd71617c998b4ce15407203218b6a8d798ad8f1c81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43256380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a760a11bc28340f784cd5eba88768f2591616ffeb26a507c49424a66826bd1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:18 GMT
ADD file:80b46be2fe86b402518b00758ff5d8556d92113dc267a002b6c72a5f9c6742a3 in / 
# Tue, 19 Jul 2022 22:20:18 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 22:37:11 GMT
ARG version=8.342.07.1
# Tue, 19 Jul 2022 22:37:20 GMT
# ARGS: version=8.342.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Tue, 19 Jul 2022 22:37:21 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:37:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:decfdc335d9bae9ca06166e1a4fc2cdf8c2344a42d85c8a1d3f964aab59ecff5`  
		Last Modified: Tue, 19 Jul 2022 22:20:55 GMT  
		Size: 2.8 MB (2818512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d446f7751415c092389678df455f15b06ffbdf495379e86716e83071f8a1d82`  
		Last Modified: Tue, 19 Jul 2022 22:43:21 GMT  
		Size: 40.4 MB (40437868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
