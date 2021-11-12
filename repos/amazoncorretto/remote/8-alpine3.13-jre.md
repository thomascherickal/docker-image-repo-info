## `amazoncorretto:8-alpine3.13-jre`

```console
$ docker pull amazoncorretto@sha256:e23a9e550df83de7707292c65691df5792c182c0690963661cc961a71e88730e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.13-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5bbdc18af90a6d54b50a9fd7b99c640a0c74b39d738118f8a7488433f4dbaaab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43175063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb5299bd2d140b3b3f9745be7f1b989b8fe721aa979640d0e3dfc2614bf5027a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:18:43 GMT
ARG version=8.312.07.1
# Fri, 12 Nov 2021 21:18:55 GMT
# ARGS: version=8.312.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Fri, 12 Nov 2021 21:18:55 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:18:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8accce84a78dd335f132829893cb1f48f7b627b9fae80bb4161e8730803942d`  
		Last Modified: Fri, 12 Nov 2021 21:23:51 GMT  
		Size: 40.4 MB (40352638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
