## `golang:nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:fa928fbb2220fb262c353833db5f627a3efedffeb5dfe35da3371c668adcf11f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1366; amd64

### `golang:nanoserver-ltsc2022` - windows version 10.0.20348.1366; amd64

```console
$ docker pull golang@sha256:bbe993450f9241bcedf6ff32ecf78cb905ef80d0467ea8a90f2802aedc76708f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279584508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9a37e61cc1d7d1e0b7ba7da094dcac8d55e8afa696b8c4fd65d1b10ef21303`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 09 Dec 2022 09:19:21 GMT
RUN Apply image 10.0.20348.1366
# Wed, 14 Dec 2022 00:26:31 GMT
SHELL [cmd /S /C]
# Wed, 14 Dec 2022 00:26:32 GMT
ENV GOPATH=C:\go
# Wed, 14 Dec 2022 00:26:33 GMT
USER ContainerAdministrator
# Wed, 14 Dec 2022 00:27:24 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 14 Dec 2022 00:27:25 GMT
USER ContainerUser
# Wed, 11 Jan 2023 00:08:24 GMT
ENV GOLANG_VERSION=1.19.5
# Wed, 11 Jan 2023 00:10:56 GMT
COPY dir:10c8e524c1346a2fb1d71240899f8be8a5c84e42a02e32a993c68761bb742a41 in C:\Program Files\Go 
# Wed, 11 Jan 2023 00:11:26 GMT
RUN go version
# Wed, 11 Jan 2023 00:11:27 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:70d3e1cc3b0ea172dcc93064fe6fb9f1f2c8fec6962c90e39991fe89a3c1ca03`  
		Last Modified: Wed, 14 Dec 2022 00:08:13 GMT  
		Size: 122.1 MB (122108200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f9e07f68da133ce8f348b35ab3af5ec6b757880ed6c11fe2b1e180d9cc11d2`  
		Last Modified: Wed, 14 Dec 2022 01:13:28 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e81455d58d6302713c7c2894d623cf87fbdb77bdd7986dfad55d2c1e581cb50`  
		Last Modified: Wed, 14 Dec 2022 01:13:27 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1be4091c182a3ccdc3f5d2c6ea93feafc2c6f9f3b18a682ccad2b6ffb87f55`  
		Last Modified: Wed, 14 Dec 2022 01:13:27 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb445693a238338ac113b54e5e1ac0344856cb2616d9d326cd0d046c1d51f8b0`  
		Last Modified: Wed, 14 Dec 2022 01:13:27 GMT  
		Size: 87.8 KB (87779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ac4511a7a13aad36c55a669c7c2931758cc1a3315a92622dcfb3c57b7d3966`  
		Last Modified: Wed, 14 Dec 2022 01:13:25 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbf5fc5dc2959a5516c441366b483f1ddf367304ad799a0490816fa688a392c`  
		Last Modified: Wed, 11 Jan 2023 00:36:03 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cb26c2de7b8c04679ddc31a7b283b0e129bc42382dfe21e1154ac3af05a7fa`  
		Last Modified: Wed, 11 Jan 2023 00:37:01 GMT  
		Size: 157.3 MB (157332270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28eedaaa0969602e640fae771c6732869099d28d6db9024f510148cd45b26e4`  
		Last Modified: Wed, 11 Jan 2023 00:36:03 GMT  
		Size: 49.1 KB (49081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea516200f33d639dc9c34b7cca974a7bc33bd5c61ed7b155d01fcd4931a39648`  
		Last Modified: Wed, 11 Jan 2023 00:36:03 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
