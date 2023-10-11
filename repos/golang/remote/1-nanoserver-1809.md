## `golang:1-nanoserver-1809`

```console
$ docker pull golang@sha256:58cf6770f8f7dc74f5730030e428fc95c0c162e96b75f3c039f635a1b0541371
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `golang:1-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull golang@sha256:76d40d568563d55e679da0cdc76ed3adc513dee9b3c19c919e517006131c1a8c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.6 MB (173646574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e8415f782312faf8fc0cd3058f8ce812e34ec94e7b0070325590824be30a5fd`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 02:31:25 GMT
SHELL [cmd /S /C]
# Wed, 11 Oct 2023 02:31:26 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:31:26 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 02:31:34 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 11 Oct 2023 02:31:35 GMT
USER ContainerUser
# Wed, 11 Oct 2023 02:31:35 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:33:25 GMT
COPY dir:af619581ed50e9a9022bf0c987a1da2c20aafc1c50d911f1206fcd3d4c232de2 in C:\Program Files\Go 
# Wed, 11 Oct 2023 02:33:41 GMT
RUN go version
# Wed, 11 Oct 2023 02:33:42 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1d090bf86f6024502bc8f94ffdf6082818dc40adde892065acecc65617301f`  
		Last Modified: Wed, 11 Oct 2023 02:48:49 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3899c15307371798776a6d43365898f31d30219b778a1f786548afe6c8dcaa`  
		Last Modified: Wed, 11 Oct 2023 02:48:49 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59029532b95f3b533c047112c719ce773b17fbeec0e514fc3979eeeb6f9d6272`  
		Last Modified: Wed, 11 Oct 2023 02:48:49 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec302bb5318ed09da9f05ac306ed7aed616e99be68aefc269e1ba6edeaf8e541`  
		Last Modified: Wed, 11 Oct 2023 02:48:49 GMT  
		Size: 70.2 KB (70154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f68a13e579f712cfba3560b02450af2ddb4adb03c25470dfac25e7b4cabd46`  
		Last Modified: Wed, 11 Oct 2023 02:48:47 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3640006b58ebd99871460915485e38d01fe7bbb0f89a5cf4a59b1e72e73465`  
		Last Modified: Wed, 11 Oct 2023 02:48:47 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f7f4ad1d0edcc52d1153d7f51a055453e890e6076b0b1f5f9ea37ca3cdf82b`  
		Last Modified: Wed, 11 Oct 2023 02:49:11 GMT  
		Size: 69.0 MB (69028060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e53bf4f074d17f2a22716ec05913bee34eb9b701be39acc272f337c5cfaacb`  
		Last Modified: Wed, 11 Oct 2023 02:48:47 GMT  
		Size: 76.9 KB (76872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322a2db63c36de055e1d5544be2fd6066eb29f318417608234d2d8fe0e60023b`  
		Last Modified: Wed, 11 Oct 2023 02:48:47 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
