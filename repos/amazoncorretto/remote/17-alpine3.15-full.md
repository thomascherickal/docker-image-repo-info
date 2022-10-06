## `amazoncorretto:17-alpine3.15-full`

```console
$ docker pull amazoncorretto@sha256:cf8fb6e70d128822fdcb2353b41f2613c0475bc3c87803677f1448f2247687d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.15-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e3c481140031755f25acb69f6025115cc182054c96dbc08aa58574630b4033cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194485518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbc6baa14d8b0f44284bad9f89e8c29317c143567508d3560fc46835a77f0e32`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:36:23 GMT
ARG version=17.0.4.9.1
# Thu, 06 Oct 2022 19:36:29 GMT
# ARGS: version=17.0.4.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Thu, 06 Oct 2022 19:36:29 GMT
ENV LANG=C.UTF-8
# Thu, 06 Oct 2022 19:36:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 06 Oct 2022 19:36:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999d431917396afee82570c75bf80b4f4e5d1d1deaf0a1025de462f83bfb412f`  
		Last Modified: Thu, 06 Oct 2022 19:46:09 GMT  
		Size: 191.7 MB (191662006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
