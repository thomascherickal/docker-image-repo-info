## `amazoncorretto:11-alpine3.14-full`

```console
$ docker pull amazoncorretto@sha256:9180ed98533f977b68a31225ba6a1f34306dfbb32feadd4f8d4e10315c200b59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine3.14-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:fabb43b1d45c6fd5d3dc8b4545dab0bbd2b6aaa691ee5c845d37d347f9bcce91
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.0 MB (196030948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33bf3157809aa4f633ddf384a1a2fd7357a59787aefcff8872b38dfbc85c667`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:18 GMT
ADD file:80b46be2fe86b402518b00758ff5d8556d92113dc267a002b6c72a5f9c6742a3 in / 
# Tue, 19 Jul 2022 22:20:18 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 22:38:14 GMT
ARG version=11.0.16.8.1
# Tue, 19 Jul 2022 22:38:20 GMT
# ARGS: version=11.0.16.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 19 Jul 2022 22:38:21 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:38:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Jul 2022 22:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:decfdc335d9bae9ca06166e1a4fc2cdf8c2344a42d85c8a1d3f964aab59ecff5`  
		Last Modified: Tue, 19 Jul 2022 22:20:55 GMT  
		Size: 2.8 MB (2818512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7a3095d2ff9f199a65844cfdf569ecb983c47096400755517a9745eaf4f962`  
		Last Modified: Tue, 19 Jul 2022 22:45:30 GMT  
		Size: 193.2 MB (193212436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
