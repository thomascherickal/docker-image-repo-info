## `golang:1-nanoserver-1809`

```console
$ docker pull golang@sha256:4eaf951b8e8db924472a4e0918d202029f9dcb05b6d90f9dba6f248482a2e2c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4851; amd64

### `golang:1-nanoserver-1809` - windows version 10.0.17763.4851; amd64

```console
$ docker pull golang@sha256:a80631f7fa07e7e9106e4c44452d44bb3448948b5a15ce4156debfc5381ccdbb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173706375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46776fec76b6969d5d075a2a62c1810045cc552be661e5647b8f7a871dfd4abe`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 01:47:57 GMT
SHELL [cmd /S /C]
# Wed, 13 Sep 2023 01:47:58 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:47:58 GMT
USER ContainerAdministrator
# Wed, 13 Sep 2023 01:48:11 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 13 Sep 2023 01:48:11 GMT
USER ContainerUser
# Thu, 05 Oct 2023 21:22:17 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:23:48 GMT
COPY dir:9ccc2bf7002ab33c0e3cb58548b90c047d0be2503f18c738ca4de2990ff1b8eb in C:\Program Files\Go 
# Thu, 05 Oct 2023 21:23:58 GMT
RUN go version
# Thu, 05 Oct 2023 21:23:58 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bbcbc05a0b3c240fc185ae93c7d844ad01c0d60ef9429ad4d230a78065a9ce`  
		Last Modified: Wed, 13 Sep 2023 02:18:48 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1e526c765b27c72087e9a2128ea7b6b61fc77a68cd2b262fc4a2ab707c796a`  
		Last Modified: Wed, 13 Sep 2023 02:18:48 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58460b34cb3f67b053b2e549f885cb1e1f16bf93c664b9cff07b3be1f5df9bf1`  
		Last Modified: Wed, 13 Sep 2023 02:18:48 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f49a4f5db38c7a1ef78003f7cb98be0df3b68ca1a1f9f5b846f8448579e643e`  
		Last Modified: Wed, 13 Sep 2023 02:18:48 GMT  
		Size: 69.8 KB (69767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf36275e1acbd42fa13589661b8d8766a7fa47d340e9e0779f3d7387ea972e4`  
		Last Modified: Wed, 13 Sep 2023 02:18:46 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77a61a1713ec43bffd5cdde2d7e5854fde8ef5950d8f9d115fed3d42f394142`  
		Last Modified: Thu, 05 Oct 2023 21:35:57 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a423cb968803cc96a9781996a01284671ec7614774469083852ccac3f87fccf`  
		Last Modified: Thu, 05 Oct 2023 21:36:13 GMT  
		Size: 69.1 MB (69063084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf60224c0415e8c262dc9df75aab216a45f9f1b9641ea6a5029e8cb6acf107a`  
		Last Modified: Thu, 05 Oct 2023 21:35:57 GMT  
		Size: 74.0 KB (73951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4601af19364383dcc9513579c98bd93c0dfdc79eca44396b9364b03d4dd89476`  
		Last Modified: Thu, 05 Oct 2023 21:35:57 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
