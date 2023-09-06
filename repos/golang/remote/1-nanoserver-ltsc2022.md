## `golang:1-nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:9bd5f1bc18ae4e8d54fe88d0c859dd782ac7f9073f8336769bf297f0c35735ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `golang:1-nanoserver-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull golang@sha256:4f94d9f49ceab50feee680652f67ad06621f50c6ce66be7b81fd722a88c33425
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.7 MB (189702604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81a66f9ca18689d381fb7d0f6566314eaae02bd60972dc439a8742e643f907da`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 03 Aug 2023 09:40:19 GMT
RUN Apply image 10.0.20348.1906
# Thu, 10 Aug 2023 00:45:25 GMT
SHELL [cmd /S /C]
# Thu, 10 Aug 2023 00:45:25 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:45:26 GMT
USER ContainerAdministrator
# Thu, 10 Aug 2023 00:45:41 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Thu, 10 Aug 2023 00:45:42 GMT
USER ContainerUser
# Wed, 06 Sep 2023 18:36:56 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:38:39 GMT
COPY dir:be682b819fc6157c5849876d4d281ecc9c26fd804e58407c442594a19c48910f in C:\Program Files\Go 
# Wed, 06 Sep 2023 18:38:59 GMT
RUN go version
# Wed, 06 Sep 2023 18:39:00 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:ea9613880997b3ab2284a37c0c14a403553457b0c331b41c6bd6d1cc7838a222`  
		Last Modified: Tue, 08 Aug 2023 18:47:21 GMT  
		Size: 120.5 MB (120500677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a528e77cf0bef98e15c3b4194ee340960485498ac4c1bdcbab44307858ecfc4`  
		Last Modified: Thu, 10 Aug 2023 01:03:26 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4287adcc177140a1d49ede9aba58d0e4266daff7899156f821c228ff5e26e4`  
		Last Modified: Thu, 10 Aug 2023 01:03:26 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165623060fccc8fd72ac1aee74f9dec194514da3ad631a694c4dadd39a7efc93`  
		Last Modified: Thu, 10 Aug 2023 01:03:26 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41934ff5e4a1f7de6165371bf05245eba59f79a718a0e4c63b0c1272984e97a`  
		Last Modified: Thu, 10 Aug 2023 01:03:26 GMT  
		Size: 77.2 KB (77192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766ddc6fd21c9745584f53d5f3ae272f830b0f0fed2455fc7c84ce55600a2b0`  
		Last Modified: Thu, 10 Aug 2023 01:03:24 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad8424c4c67340163a45617eecb90138d544b937186ee8f1d4417c514c3beda`  
		Last Modified: Wed, 06 Sep 2023 18:53:56 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255342497af82dfdc57587650ca2ad486aa1807cdf8f1860910f8dc86b55446f`  
		Last Modified: Wed, 06 Sep 2023 18:54:14 GMT  
		Size: 69.1 MB (69064630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720bb624a439341f77e1603a51fa2e91643f63f675d94ed4ca39470ac0f6ab1`  
		Last Modified: Wed, 06 Sep 2023 18:53:57 GMT  
		Size: 53.0 KB (52986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648dbc37c5afd164e235c58f9d9fa8b2e3af18fb60496172b709f3d935c32a3a`  
		Last Modified: Wed, 06 Sep 2023 18:53:57 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
