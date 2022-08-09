## `amazoncorretto:8-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:479c005d667854748b061b722923a72fe1d60fa71a3059bb3ae829b4a829e4ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:2b953b2b1af25779527210eb4a5337a8c35b3ec667026a8667f62045b807979b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101620885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fda0f570093397feb33c5f2548b1554ceb67d3250679e970b0210fb3bf4db501`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:37:16 GMT
ARG version=8.342.07.4
# Tue, 09 Aug 2022 17:37:20 GMT
# ARGS: version=8.342.07.4
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 09 Aug 2022 17:37:21 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 17:37:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 09 Aug 2022 17:37:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d387ba25a0ffcec6f01a449b245ffbc4605b69bf58d703c93f0a42bd9ac7f10`  
		Last Modified: Tue, 09 Aug 2022 17:41:59 GMT  
		Size: 98.8 MB (98797373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
