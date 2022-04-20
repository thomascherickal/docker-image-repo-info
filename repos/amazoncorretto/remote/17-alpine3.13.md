## `amazoncorretto:17-alpine3.13`

```console
$ docker pull amazoncorretto@sha256:2a40b3d1f6a7fbf959db422419a24c272e5e35f888c54693e62ff3e3ebd4a59c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.13` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:75fa359ea41d35476c12b82e64356e8c50134536c25615bc85a5dbbe6b53c3f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194749361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d28e8f32086e79ca3ddd23825fbf05b4e7bd49fb5489a375a2b9523a06c64db4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 22:25:37 GMT
ARG version=17.0.3.6.1
# Tue, 19 Apr 2022 22:25:43 GMT
# ARGS: version=17.0.3.6.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Tue, 19 Apr 2022 22:25:43 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:25:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Apr 2022 22:25:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d69297464837423fd0c5f6bb49969d9359131154a5907578ba999a043dffe1`  
		Last Modified: Tue, 19 Apr 2022 22:35:57 GMT  
		Size: 191.9 MB (191930049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
