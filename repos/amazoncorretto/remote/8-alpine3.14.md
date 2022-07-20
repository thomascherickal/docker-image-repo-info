## `amazoncorretto:8-alpine3.14`

```console
$ docker pull amazoncorretto@sha256:d8e0915dabe4484ef728f3cb9dafd1b858df55b4d9cb02192afc07998cf7f761
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.14` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6c10d64e7d6efee6765e2d49211f966469e732305f5894e1ade4bc69530e6508
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101618467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf4adf1d6b80a4371dd72129ad81dc7e04b2606421ac7aacbb6e0ae5b16bedd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:18 GMT
ADD file:80b46be2fe86b402518b00758ff5d8556d92113dc267a002b6c72a5f9c6742a3 in / 
# Tue, 19 Jul 2022 22:20:18 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 22:37:11 GMT
ARG version=8.342.07.1
# Tue, 19 Jul 2022 22:37:15 GMT
# ARGS: version=8.342.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 19 Jul 2022 22:37:15 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:37:15 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Jul 2022 22:37:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:decfdc335d9bae9ca06166e1a4fc2cdf8c2344a42d85c8a1d3f964aab59ecff5`  
		Last Modified: Tue, 19 Jul 2022 22:20:55 GMT  
		Size: 2.8 MB (2818512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231fd7c2b53cb5ff6343b025f1620486d6bb31730e9b5ec2da699a5a92f00b50`  
		Last Modified: Tue, 19 Jul 2022 22:43:03 GMT  
		Size: 98.8 MB (98799955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
