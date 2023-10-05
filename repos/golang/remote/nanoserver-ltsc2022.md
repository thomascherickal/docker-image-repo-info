## `golang:nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:7397357059a23a1eac0413b413bce60358ff4de6eadc9acc8e632b5c79720682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `golang:nanoserver-ltsc2022` - windows version 10.0.20348.1970; amd64

```console
$ docker pull golang@sha256:778b4cc358c5a3fc76d82df4a1171b48785831897b0027d85312a8d510e228f3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.8 MB (189772835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02450fbb0e6c0e79e1369b9e471642b48952965a69f6a48248f78b5dd9b76954`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 01 Sep 2023 00:20:14 GMT
RUN Apply image 10.0.20348.1970
# Wed, 13 Sep 2023 01:45:13 GMT
SHELL [cmd /S /C]
# Wed, 13 Sep 2023 01:45:13 GMT
ENV GOPATH=C:\go
# Wed, 13 Sep 2023 01:45:14 GMT
USER ContainerAdministrator
# Wed, 13 Sep 2023 01:45:30 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 13 Sep 2023 01:45:30 GMT
USER ContainerUser
# Thu, 05 Oct 2023 21:20:05 GMT
ENV GOLANG_VERSION=1.21.2
# Thu, 05 Oct 2023 21:21:46 GMT
COPY dir:9ccc2bf7002ab33c0e3cb58548b90c047d0be2503f18c738ca4de2990ff1b8eb in C:\Program Files\Go 
# Thu, 05 Oct 2023 21:21:57 GMT
RUN go version
# Thu, 05 Oct 2023 21:21:57 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:8f8cef0759210af9d01a2fb45d79956a2db738bbd3734b7244b17e14ad945cab`  
		Last Modified: Tue, 12 Sep 2023 18:47:39 GMT  
		Size: 120.6 MB (120567584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c795bb9d48e9fa247e549604525fcb2599507cf1008aa1df12036f428ea236d`  
		Last Modified: Wed, 13 Sep 2023 02:18:07 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfefaf16c2467f3b414f23f271a0b3500e0e6e4b5a6c283d9d4504942bb41d0b`  
		Last Modified: Wed, 13 Sep 2023 02:18:07 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8af5eba6c23e059dfc62ac724d10f9b02be442608028bed7e0439b86b148da`  
		Last Modified: Wed, 13 Sep 2023 02:18:07 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b58761750bd8ba8ee22556e6be99c30963fbac0e030c41564ed881a6a80fcf`  
		Last Modified: Wed, 13 Sep 2023 02:18:07 GMT  
		Size: 80.9 KB (80890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c227eff309d8eb3e6b97da880ffba88c776a248aa79e78574def6dd088dbe6f7`  
		Last Modified: Wed, 13 Sep 2023 02:18:05 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f8228793d3e9494bbe5ffebe22c0872dd22776723eddbfddd7337bc31b61cc`  
		Last Modified: Thu, 05 Oct 2023 21:35:25 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd61489b33322cb77de580c31f7a2a1e289500663e2a99a9e51e521bc1a882b`  
		Last Modified: Thu, 05 Oct 2023 21:35:40 GMT  
		Size: 69.1 MB (69057749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59d8fcb657011c9fe0489908997bae37f9aebc203d86507e75e2ed2f29fbb96`  
		Last Modified: Thu, 05 Oct 2023 21:35:25 GMT  
		Size: 59.4 KB (59446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31201668444e4cec46113bb9f765b6803dc6fdc9d997ad72cd22461effda04f4`  
		Last Modified: Thu, 05 Oct 2023 21:35:25 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
