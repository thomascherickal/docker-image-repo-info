## `amazoncorretto:17-alpine3.15-full`

```console
$ docker pull amazoncorretto@sha256:b6e7ee3e1f2b8c59d4b9fec3a2b54e2645fd9d80c1df330b1f8f99ec063765d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.15-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:fb2d1dca574228296a738e11acc11264e77ffdacad8a0420f0a9cfe6d4a3ad92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194485614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d00013d63ffc84cd001b039f08823bfa000c279bfd33b20240dc9b86ef659f1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 16 Aug 2022 23:21:36 GMT
ARG version=17.0.4.9.1
# Tue, 16 Aug 2022 23:21:42 GMT
# ARGS: version=17.0.4.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Tue, 16 Aug 2022 23:21:43 GMT
ENV LANG=C.UTF-8
# Tue, 16 Aug 2022 23:21:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 16 Aug 2022 23:21:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b870c08a78c6304ee7971a65c6153cc957829187674bc57448487a87fd273b`  
		Last Modified: Tue, 16 Aug 2022 23:27:15 GMT  
		Size: 191.7 MB (191662102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
