## `amazoncorretto:17-alpine3.14`

```console
$ docker pull amazoncorretto@sha256:506b34482acb364989a87c6f97f9301c4e064f2225ab7e68f9e6d167b1fadee5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.14` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:3ccdeaa349971e591585f84b8fb05e86da83b5a2bdeed58f9bd483eed546040f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194486148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f41d2a317c640ccc3e994697422c4f0e7f1f5bc9ee462f1835918e9a5ce3c3c5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:18 GMT
ADD file:80b46be2fe86b402518b00758ff5d8556d92113dc267a002b6c72a5f9c6742a3 in / 
# Tue, 19 Jul 2022 22:20:18 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 22:39:13 GMT
ARG version=17.0.4.8.1
# Tue, 19 Jul 2022 22:39:19 GMT
# ARGS: version=17.0.4.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Tue, 19 Jul 2022 22:39:19 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:39:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Jul 2022 22:39:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:decfdc335d9bae9ca06166e1a4fc2cdf8c2344a42d85c8a1d3f964aab59ecff5`  
		Last Modified: Tue, 19 Jul 2022 22:20:55 GMT  
		Size: 2.8 MB (2818512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e851542186e768bd29be61c9244aa68f842cae86a236bc9c2b0057e82385a733`  
		Last Modified: Tue, 19 Jul 2022 22:47:34 GMT  
		Size: 191.7 MB (191667636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
