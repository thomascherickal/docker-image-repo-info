## `amazoncorretto:8-alpine3.12-jre`

```console
$ docker pull amazoncorretto@sha256:194ba48bd933d08ae25ac70cd945695be946c1290709d8e85f6d77a3a30fb880
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.12-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:f5308d8d67a303e8cb1ef37e8d5973f8e6cdd5584cb6dc2be33dcdccc47f9ca4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43149754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a694f896151049eacf27770741a8298a444bfa342cc490d54d33bfdce087c9f8`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:30:26 GMT
ARG version=8.302.08.1
# Wed, 01 Sep 2021 00:30:44 GMT
# ARGS: version=8.302.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Wed, 01 Sep 2021 00:30:45 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 00:30:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123dc5594dbc3dde316acc44a6ee7ec1ecbcb40b936dc192d2fe06fb8e53df18`  
		Last Modified: Wed, 01 Sep 2021 00:32:56 GMT  
		Size: 40.3 MB (40348047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
