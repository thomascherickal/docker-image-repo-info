## `amazoncorretto:8-alpine3.14-jdk`

```console
$ docker pull amazoncorretto@sha256:8f1b86a6581765b0a9ed49cd2eb8f947bb2eb85dfc97ffcb5ad9e3cf7d6f1d04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.14-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5874eec592db8dc5c6880b78d20aaa3aba595e71eed2bba3b9d19004b4350ad4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101615876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a26f3a8c5f8218ebfea6a7ccff9bf907aac067ad60e32a5f1ca2c10bac5251af`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:18 GMT
ADD file:80b46be2fe86b402518b00758ff5d8556d92113dc267a002b6c72a5f9c6742a3 in / 
# Tue, 19 Jul 2022 22:20:18 GMT
CMD ["/bin/sh"]
# Fri, 29 Jul 2022 20:20:14 GMT
ARG version=8.342.07.4
# Fri, 29 Jul 2022 20:20:18 GMT
# ARGS: version=8.342.07.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Fri, 29 Jul 2022 20:20:18 GMT
ENV LANG=C.UTF-8
# Fri, 29 Jul 2022 20:20:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 29 Jul 2022 20:20:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:decfdc335d9bae9ca06166e1a4fc2cdf8c2344a42d85c8a1d3f964aab59ecff5`  
		Last Modified: Tue, 19 Jul 2022 22:20:55 GMT  
		Size: 2.8 MB (2818512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce486913adcbdabddbf3baf82c6487d0d53a5c853b27783d875229b983efc1`  
		Last Modified: Fri, 29 Jul 2022 20:23:45 GMT  
		Size: 98.8 MB (98797364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
