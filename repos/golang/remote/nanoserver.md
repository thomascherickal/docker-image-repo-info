## `golang:nanoserver`

```console
$ docker pull golang@sha256:11b1bc2a66d213de58852d57ad0cdc7ecad54bee77624834e8ab2dd264904873
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `golang:nanoserver` - windows version 10.0.20348.2031; amd64

```console
$ docker pull golang@sha256:16c614276387fcc4dd88600c7541b937533aa4d68a89507b5d56d816a1add074
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.8 MB (189764917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d06c4c2afa2069f6b273ddc38811a59ada5d4fae2c940c8190aaadf20166bb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:28:41 GMT
SHELL [cmd /S /C]
# Wed, 11 Oct 2023 02:28:42 GMT
ENV GOPATH=C:\go
# Wed, 11 Oct 2023 02:28:43 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 02:28:54 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 11 Oct 2023 02:28:54 GMT
USER ContainerUser
# Wed, 11 Oct 2023 02:28:55 GMT
ENV GOLANG_VERSION=1.21.3
# Wed, 11 Oct 2023 02:30:48 GMT
COPY dir:af619581ed50e9a9022bf0c987a1da2c20aafc1c50d911f1206fcd3d4c232de2 in C:\Program Files\Go 
# Wed, 11 Oct 2023 02:31:08 GMT
RUN go version
# Wed, 11 Oct 2023 02:31:09 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:fff54800e03713ba81736f43d985319592fc643a1a32b62dbd5c0ec36549de00`  
		Last Modified: Tue, 10 Oct 2023 17:30:43 GMT  
		Size: 120.6 MB (120604344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54cd425f94dc5addd6f49003c495c9acbf2a61ab29ca68946c6cd056ed33c5f6`  
		Last Modified: Wed, 11 Oct 2023 02:48:05 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f6380212a72bc3e40c69e29ce0d1231ecc69a9b706d901e4b7f9aef73239e`  
		Last Modified: Wed, 11 Oct 2023 02:48:05 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f6b265e014a5bbb4382fcfdd5bff58743fb56e3b22627bed9ea923b9c32c40`  
		Last Modified: Wed, 11 Oct 2023 02:48:05 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720973e6116d7650d6e62cd18f427c31ba73fffd89e2494d2dac217e7a77e071`  
		Last Modified: Wed, 11 Oct 2023 02:48:05 GMT  
		Size: 74.9 KB (74931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3532145af5012419fa25862c2d443a7cca3651123589d4478bfe1a9ec6d74b4a`  
		Last Modified: Wed, 11 Oct 2023 02:48:03 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762bf66d041866ee37bd607c6e66a0fdab7dc8753c3250a09a598b13b77bc3ab`  
		Last Modified: Wed, 11 Oct 2023 02:48:03 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5905c1e4b160f74287977cfc13c889335f02d27e7547ed8b11b61bafc4b16fae`  
		Last Modified: Wed, 11 Oct 2023 02:48:28 GMT  
		Size: 69.0 MB (69027894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb1d98ff90903510b010a70e4f72f4e60339fbd2bfe75b91e303a2bebe6d846`  
		Last Modified: Wed, 11 Oct 2023 02:48:03 GMT  
		Size: 51.2 KB (51188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff590871d176c43caa3fa01c551e4f62ab8b74505ec678a46b0496db1d4ea7ba`  
		Last Modified: Wed, 11 Oct 2023 02:48:03 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:nanoserver` - windows version 10.0.17763.4974; amd64

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
