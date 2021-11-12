## `amazoncorretto:17-alpine3.12-jdk`

```console
$ docker pull amazoncorretto@sha256:aba50355829acd7490b4ec18766a5596260688efa6bdb7751b83032a2370ceb1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.12-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:2b948bcc498621ebe6ea71330cc3db4b6507fe1737ca01aa6aad2d3d5dda9af1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194568900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c168d09729b913550aa5ef2280782f5a9f33fed658beadf7e621e0a32e27118d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:19:49 GMT
ARG version=17.0.1.12.1
# Fri, 12 Nov 2021 21:19:57 GMT
# ARGS: version=17.0.1.12.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Fri, 12 Nov 2021 21:19:58 GMT
ENV LANG=C.UTF-8
# Fri, 12 Nov 2021 21:19:58 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Fri, 12 Nov 2021 21:19:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7a041600fca1719e4b9c09f02d77594b75b35389da824269524e4d40c698f3`  
		Last Modified: Fri, 12 Nov 2021 21:27:04 GMT  
		Size: 191.8 MB (191759427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
