## `amazoncorretto:19-alpine3.15-jdk`

```console
$ docker pull amazoncorretto@sha256:98f429d25f4b45f95d898fbce0aa3459edd7a0b2a8952a7b076cd222f97ecc06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:19-alpine3.15-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f032a0b19cf69edd41ef3e0969c8b2719598bfd9d66ca37fe6d6cddde484bc7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.0 MB (203038398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ed40d109f639150fb4a81049ff830d7b09dc20b2a34c3328d3f97cec887f6d5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:37:51 GMT
ARG version=19.0.0.36.1
# Thu, 06 Oct 2022 19:37:57 GMT
# ARGS: version=19.0.0.36.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-19=$version-r0
# Thu, 06 Oct 2022 19:37:58 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 19:37:58 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 06 Oct 2022 19:37:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1378a94fa16157598279911e6934034bf9008145356465269f6bbb6655308d38`  
		Last Modified: Thu, 06 Oct 2022 19:50:19 GMT  
		Size: 200.2 MB (200214886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
