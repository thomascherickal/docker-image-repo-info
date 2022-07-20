## `amazoncorretto:8-alpine3.13-jre`

```console
$ docker pull amazoncorretto@sha256:f10b36a9274fb44bd2cf4c4ba54c64fab71573350ccf8ec74eb0fef1411c558a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.13-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:29ad8600bb4a2b62215042b6167c15273cbaa0269dbda2ec453bcc3f3fef6b0d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43255543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea6cfc8e951ec04824f3f2c97cca51b070dad7427b8331ea9159645d2cd659f5`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:26 GMT
ADD file:e15461ac94648d9599df6304a53587fc8bfceaf6e111ee5917860e95ed9e751c in / 
# Tue, 19 Jul 2022 22:20:26 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 22:36:57 GMT
ARG version=8.342.07.1
# Tue, 19 Jul 2022 22:37:08 GMT
# ARGS: version=8.342.07.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Tue, 19 Jul 2022 22:37:08 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:37:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:627fad6f28f79c3907ad18a4399be4d810c0e1bb503fe3712217145c555b9d2f`  
		Last Modified: Tue, 19 Jul 2022 22:21:04 GMT  
		Size: 2.8 MB (2819330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90d7069b17c44f0b3092f1cc85327bde210900f55fbbcad2569b46f628a335a`  
		Last Modified: Tue, 19 Jul 2022 22:42:44 GMT  
		Size: 40.4 MB (40436213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
