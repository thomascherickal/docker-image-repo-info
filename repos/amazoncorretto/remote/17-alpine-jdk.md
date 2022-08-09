## `amazoncorretto:17-alpine-jdk`

```console
$ docker pull amazoncorretto@sha256:952587335b970878cbca78f6ba888c32c51c8ae70b1ef76ca5864c8d93b23d49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d11eaf0c564378e1013a4ac908896a0dd54a898da6b1622b07cc37f9bdbfc2b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194491226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ef4de872658b05415949a42bd4067586896be896b6bfa48e9f8e300968a25a8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:28 GMT
ARG version=17.0.4.8.1
# Tue, 09 Aug 2022 17:38:34 GMT
# ARGS: version=17.0.4.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Tue, 09 Aug 2022 17:38:34 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 17:38:35 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 09 Aug 2022 17:38:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9c8d9aa8ac7a5ab19fa2e13695f8d07c25fbea0373192592457fb9ecc1aba3`  
		Last Modified: Tue, 09 Aug 2022 17:45:33 GMT  
		Size: 191.7 MB (191667714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
