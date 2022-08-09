## `amazoncorretto:17-alpine3.14-full`

```console
$ docker pull amazoncorretto@sha256:e757471a75443ef7191dc2b6eca524320f8b6cd5799879575d67fb03769d56d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.14-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:08f238af8556b8aa8da6420c1e7999f82a1f5e16fe18f9a9661cb9215919059d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194495072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f23d08eab8b081835cbc2d1ef396236e94ae9ff1ffe88c81727e09013889202`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:18 GMT
ARG version=17.0.4.8.1
# Tue, 09 Aug 2022 17:38:24 GMT
# ARGS: version=17.0.4.8.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Tue, 09 Aug 2022 17:38:25 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 17:38:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 09 Aug 2022 17:38:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75504932243d3912529f1ca2f01d003912a7f004864f8b1ea7a432c72463cded`  
		Last Modified: Tue, 09 Aug 2022 17:45:04 GMT  
		Size: 191.7 MB (191667583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
