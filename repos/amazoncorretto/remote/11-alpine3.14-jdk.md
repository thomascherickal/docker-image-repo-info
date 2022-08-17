## `amazoncorretto:11-alpine3.14-jdk`

```console
$ docker pull amazoncorretto@sha256:eae8ceb84d6eddf1d1272984f34efecf2fdd43b5227f606108780889b58522e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-alpine3.14-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:58ed3abaa0e1e94623315b65e6ee27478ead8596363755404ed5541a8fba93cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.0 MB (196036722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ad91ee4a079747f99445f529e4919805bb3b4bac69a7a5fc81e33be4e73ffd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:07 GMT
ADD file:b9bd10cf83356cb7281baa0fbaca5186cf27491f59eda87abe57f83a5aaf5ec1 in / 
# Tue, 09 Aug 2022 17:20:08 GMT
CMD ["/bin/sh"]
# Tue, 16 Aug 2022 23:20:20 GMT
ARG version=11.0.16.9.1
# Tue, 16 Aug 2022 23:20:29 GMT
# ARGS: version=11.0.16.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-11=$version-r0
# Tue, 16 Aug 2022 23:20:30 GMT
ENV LANG=C.UTF-8
# Tue, 16 Aug 2022 23:20:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 16 Aug 2022 23:20:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:c7ed990a2339ee598662849de4f56e2241399f5a32340c8c4a7bbd5378a12b5f`  
		Last Modified: Tue, 09 Aug 2022 17:21:06 GMT  
		Size: 2.8 MB (2827489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edfd56606ca875d5cf48b8962b215d64529352fd809331823105306de364d25`  
		Last Modified: Tue, 16 Aug 2022 23:24:42 GMT  
		Size: 193.2 MB (193209233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
