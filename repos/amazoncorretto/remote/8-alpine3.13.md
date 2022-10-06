## `amazoncorretto:8-alpine3.13`

```console
$ docker pull amazoncorretto@sha256:e70f7a71670954b4f0677cd870b8776606cab7fe7689418bfdfee41bb6e68d03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.13` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e5614a96704ec707622caac3470a19007bbd3d76145b5cd6d861b6fe2ca285e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101619539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9aba42ad30274c768497ca8981384b3397d6431bd1f527e62e447e00ab846b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:14 GMT
ADD file:7fd90c097e2c4587dee91726d71abc02fa1aa6a3a3395c862206a4e14e0c299c in / 
# Tue, 09 Aug 2022 17:20:14 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:34:26 GMT
ARG version=8.342.07.4
# Thu, 06 Oct 2022 19:34:31 GMT
# ARGS: version=8.342.07.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Thu, 06 Oct 2022 19:34:32 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 19:34:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 06 Oct 2022 19:34:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:72cfd02ff4d01b1f319eed108b53120dea0185b916d2abeb4e6121879cbf7a65`  
		Last Modified: Tue, 09 Aug 2022 17:21:16 GMT  
		Size: 2.8 MB (2827571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5917506b095a56d725ecc636e10d0e0b04ac907ff76395ae9389a0713514fe`  
		Last Modified: Thu, 06 Oct 2022 19:40:21 GMT  
		Size: 98.8 MB (98791968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
