## `golang:1-nanoserver-1809`

```console
$ docker pull golang@sha256:c1dd52f65c17f53cbf02f826732d6c283f50c47675b3393ae9a778114c41d657
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.2061; amd64

### `golang:1-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull golang@sha256:fea07128c8f7858e6d51777190d8572ee3354f183aeb58e7c2c6d69ddc85e2ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241897881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34b838f60126bb771fc0428f42ce1254ea283f7aa1f6ea69a7dcd367b828fb4f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 01:23:41 GMT
SHELL [cmd /S /C]
# Wed, 14 Jul 2021 04:39:11 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Jul 2021 04:39:14 GMT
USER ContainerAdministrator
# Wed, 14 Jul 2021 04:39:34 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Wed, 14 Jul 2021 04:39:36 GMT
USER ContainerUser
# Wed, 14 Jul 2021 04:50:06 GMT
ENV GOLANG_VERSION=1.16.6
# Wed, 14 Jul 2021 04:52:02 GMT
COPY dir:8ab75d02dd4fda59c722fe4846694761e4f44aaadc24d8b8496f1a065ed50398 in C:\go 
# Wed, 14 Jul 2021 04:52:28 GMT
RUN go version
# Wed, 14 Jul 2021 04:52:31 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5307d56ac81f33a647e0ed6f4e0f70a39b207469fe0a28ab1b9f9379669e02b4`  
		Last Modified: Wed, 14 Jul 2021 02:04:59 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d72046f3f0748f7f1cfa8143e2940c7ce6648a4092f19478ab5be051da4322`  
		Last Modified: Wed, 14 Jul 2021 05:05:15 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c01484fb96cabf37eb40789a70cb7ded860d276f0f3d67cf73c460068c4da8`  
		Last Modified: Wed, 14 Jul 2021 05:05:15 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861d147727a049b4e876c27462f827024b9faad381fdcedb6566a9dabe2686b9`  
		Last Modified: Wed, 14 Jul 2021 05:05:15 GMT  
		Size: 65.6 KB (65616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770b7cc5eaa7b215b7bf7c49e2695c7e943eaa335695c19604604130a78196e1`  
		Last Modified: Wed, 14 Jul 2021 05:05:12 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f08e881fcda7b0de5e343f59766fdd40c833e1dc87148977539d7913a793b7`  
		Last Modified: Wed, 14 Jul 2021 05:07:50 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c500beb27d5c40d6cbf77035cefc39a50a018fa31fb594770f31c1579b47f143`  
		Last Modified: Wed, 14 Jul 2021 05:08:21 GMT  
		Size: 139.0 MB (139034798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe061f64ecbf1dc553a4f528b063eaf186b5e20d4bae7805f65342d23b44743`  
		Last Modified: Wed, 14 Jul 2021 05:07:50 GMT  
		Size: 64.7 KB (64680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473bb7917ac8cd8a03710f0141647f0895239102dd12676a720bc4885b17d6df`  
		Last Modified: Wed, 14 Jul 2021 05:07:50 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
