## `amazoncorretto:8u332-alpine3.13-jre`

```console
$ docker pull amazoncorretto@sha256:d4b313101f006a1ac0ab7cce18b518575ee8a701377f85cf82a2201921bbdd14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u332-alpine3.13-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:dd6c4ee4b69b6051b6ae0902e9ec8923d5f4b0bf6eed2cb982d3f6634a847dba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43222289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4456b296d5762386e33d38b7df47ca52856af83c466616a0b261dee943e71e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 22:23:08 GMT
ARG version=8.332.08.1
# Tue, 19 Apr 2022 22:23:18 GMT
# ARGS: version=8.332.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0
# Tue, 19 Apr 2022 22:23:18 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:23:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14c4b312ae3f35e0fc1663beba7783411ae1b34c55511029ee4191bd07af8b2`  
		Last Modified: Tue, 19 Apr 2022 22:30:37 GMT  
		Size: 40.4 MB (40402977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
