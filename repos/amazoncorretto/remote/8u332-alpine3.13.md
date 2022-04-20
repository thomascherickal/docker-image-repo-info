## `amazoncorretto:8u332-alpine3.13`

```console
$ docker pull amazoncorretto@sha256:bc01dcc398cdf795050691282d8457bd4157115fec300a559e24ea1f4d83d25e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8u332-alpine3.13` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ebf1c4fdaf15b3789499f3ff233b6650dda9a2ee6d766909b3bb193e2fe4fb75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101781076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd962f2fa85af89eda8653b74a0e2885f90e65f471295f565e3dd4cb4a053616`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 22:23:08 GMT
ARG version=8.332.08.1
# Tue, 19 Apr 2022 22:23:12 GMT
# ARGS: version=8.332.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8=$version-r0
# Tue, 19 Apr 2022 22:23:13 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:23:13 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Apr 2022 22:23:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8338fb491d3e4ce77b7d5cfd0cd8de5969ebcdd385d6e6de4733005d9dcd0f48`  
		Last Modified: Tue, 19 Apr 2022 22:30:18 GMT  
		Size: 99.0 MB (98961764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
