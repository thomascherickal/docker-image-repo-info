## `amazoncorretto:8-alpine3.13-full`

```console
$ docker pull amazoncorretto@sha256:6350eebeb33fdba5071c37d206dff651b23f8c30ef7cc55ac19e21a98c995d24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.13-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:9cd4a2a65d32fbb5ea709355b2e3bf1126835d30424db9afacf442b107557a29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101607520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db0388232bdd0ea317f12eee851bb4d2b0eb3c6bded2242570ece297bed503c1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:26 GMT
ADD file:e15461ac94648d9599df6304a53587fc8bfceaf6e111ee5917860e95ed9e751c in / 
# Tue, 19 Jul 2022 22:20:26 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 22:36:57 GMT
ARG version=8.342.07.1
# Tue, 19 Jul 2022 22:37:02 GMT
# ARGS: version=8.342.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 19 Jul 2022 22:37:02 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:37:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Jul 2022 22:37:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:627fad6f28f79c3907ad18a4399be4d810c0e1bb503fe3712217145c555b9d2f`  
		Last Modified: Tue, 19 Jul 2022 22:21:04 GMT  
		Size: 2.8 MB (2819330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bd45b0d1878aca8055d5935ed0680992c9d717e0ee8b479a482d6cbfe0c185`  
		Last Modified: Tue, 19 Jul 2022 22:42:26 GMT  
		Size: 98.8 MB (98788190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
