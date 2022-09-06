## `golang:1-nanoserver`

```console
$ docker pull golang@sha256:2175f4f649b2a88dfff9254edae926ac0a3756e8c737495a707eaf0a058c771d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `golang:1-nanoserver` - windows version 10.0.20348.887; amd64

```console
$ docker pull golang@sha256:4cd5e6ac290a5d8343c726cab4690a233946db846a224bb952487825c6b98826
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275478844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40cb6b5739fa4c3cdc680f2082fd22c4a298f716a09fbc63ba631869d02b8572`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sat, 06 Aug 2022 18:05:23 GMT
RUN Apply image 10.0.20348.887
# Wed, 10 Aug 2022 13:00:01 GMT
SHELL [cmd /S /C]
# Wed, 10 Aug 2022 13:00:02 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 13:00:03 GMT
USER ContainerAdministrator
# Wed, 10 Aug 2022 13:00:52 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 10 Aug 2022 13:00:53 GMT
USER ContainerUser
# Tue, 06 Sep 2022 19:24:22 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:27:13 GMT
COPY dir:8931e4de46b22c4907fdd32bb2e3bdcb14b258c585caf020889cae248acd1241 in C:\Program Files\Go 
# Tue, 06 Sep 2022 19:28:08 GMT
RUN go version
# Tue, 06 Sep 2022 19:28:09 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:2ebf439f800cd4c1fccaf4a0545e6bff60caa5141295c8ab81f6c525073c423d`  
		Size: 118.1 MB (118088450 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:28bba27fcdd9c2f008a9c22db6c16dece3a5c3a49f9fac9447924071999adf65`  
		Last Modified: Wed, 10 Aug 2022 13:26:19 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f352dc9aa1911058088d17b0106a92f12440eeeca4743fefe0c8f4341b35cb`  
		Last Modified: Wed, 10 Aug 2022 13:26:19 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cdaa41fdd816a0d26ae34d42202146e1c097c5c1f8d4a7e89baa4b6c898e11`  
		Last Modified: Wed, 10 Aug 2022 13:26:18 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de3ee36144ab0c42283d413099bae19e983ae4415ed4f3aadf1b2f00dee77af`  
		Last Modified: Wed, 10 Aug 2022 13:26:19 GMT  
		Size: 85.0 KB (85027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd92736439907ce6bf37d9c346db5466b4a71f29695648b075e599df34b709b2`  
		Last Modified: Wed, 10 Aug 2022 13:26:16 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef41a4e2a0f3e16498f1bb0d1594baa0cdfaf6e77443d1477ccff33c32aa0c5`  
		Last Modified: Tue, 06 Sep 2022 19:50:21 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af9b83eb420c08497ed8361afa59c768b46c507c19a256aae4e93014f786912`  
		Last Modified: Tue, 06 Sep 2022 19:50:58 GMT  
		Size: 157.2 MB (157246445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bda2a58e8412c469d40a83a9109f712fe85e138cea8ed7fb7855abe7f29bcb0`  
		Last Modified: Tue, 06 Sep 2022 19:50:21 GMT  
		Size: 51.9 KB (51852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d301a857e784690c1f0651458e018f02f6446e9163446ec0090bc1000d48cb7`  
		Last Modified: Tue, 06 Sep 2022 19:50:21 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-nanoserver` - windows version 10.0.17763.3287; amd64

```console
$ docker pull golang@sha256:fc8ef4284d3e413842887d8c6510e35e5400bc04eaae2101d9f5bec7ecdfead1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.6 MB (260576155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7111777808aea55a20e3e4fe5aad7ed74e13ab814a37dfd00878081ccbae1a6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 13:04:30 GMT
SHELL [cmd /S /C]
# Wed, 10 Aug 2022 13:04:31 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 13:04:32 GMT
USER ContainerAdministrator
# Wed, 10 Aug 2022 13:05:04 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 10 Aug 2022 13:05:05 GMT
USER ContainerUser
# Tue, 06 Sep 2022 19:28:21 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:31:13 GMT
COPY dir:8931e4de46b22c4907fdd32bb2e3bdcb14b258c585caf020889cae248acd1241 in C:\Program Files\Go 
# Tue, 06 Sep 2022 19:31:59 GMT
RUN go version
# Tue, 06 Sep 2022 19:32:00 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9982991b820814ad737b2a161e973194e66b8d7b0a9890bee49cd158d7e77dec`  
		Last Modified: Wed, 10 Aug 2022 13:27:27 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb374f741579c100c895dcc59aa9485366514d2070780d936afb0cee10e2c3f6`  
		Last Modified: Wed, 10 Aug 2022 13:27:26 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732dbfa4c42c7cd3f8c88016834d3c06de0f03922e792273a4257c96c56f23b5`  
		Last Modified: Wed, 10 Aug 2022 13:27:25 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bbe06a1892b7650171a49f4f4a90a5d222516df1bf6d09c1f1cdd9d42d2188`  
		Last Modified: Wed, 10 Aug 2022 13:27:25 GMT  
		Size: 72.1 KB (72078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15263a6e39d76b9d2d60ec9ccee1249c09eb3e08cfb05422d0269497e268aeca`  
		Last Modified: Wed, 10 Aug 2022 13:27:25 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3f096e58f1bb857ddf0f2daa6368defb200ee8097b86432af9af526f2f0962`  
		Last Modified: Tue, 06 Sep 2022 19:51:13 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c94eed496ecb836eddddd841dbe69ec1a0b444b620ce1a1a6e3afa19c524ba`  
		Last Modified: Tue, 06 Sep 2022 19:51:50 GMT  
		Size: 157.3 MB (157250289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4a12fb8f08499c870be4133361a9425e78419dac4ec2088659f54f48a97f4c`  
		Last Modified: Tue, 06 Sep 2022 19:51:13 GMT  
		Size: 42.5 KB (42458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3032f59a0297718a66072e71a61d1942888b9b3a930b901ce70afeb917712b`  
		Last Modified: Tue, 06 Sep 2022 19:51:13 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
