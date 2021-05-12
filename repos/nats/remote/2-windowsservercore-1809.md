## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:92af18909a07b17d44c1b4dab108c3ec79f738445924832589a1f038531f9aa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:b8f78fa18e95ccd030921491099bdde6027366e20ac29724826806ccc57a8fc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488959507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b8a5009e27b5f8b20992ed668c1df65a85d913c82c98d32438569b82c04a87`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:41:50 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:41:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:41:52 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:42:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:43:40 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:43:42 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:43:43 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997292a293a04bf9999ffa301783c44d32ec86576fc6e0a67f833d0e3681d31`  
		Last Modified: Wed, 12 May 2021 15:48:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e994dfe884b3f7ba067e339ef8c984b37b3b677863aa953ad40d3bf4b74536`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c068dad32902ef5213f961601255c3f502986f4a52c117ce6ee6a29c14748b8a`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536fa26cb9cd7685db7d4789aeeb434b2d4429f94e1b149374cc64d27a07e5bf`  
		Last Modified: Wed, 12 May 2021 15:48:40 GMT  
		Size: 5.1 MB (5096854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882208c7ca121b0cd4752cf236a1b481d05c046c612f9674b1602c1d665d88ba`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 9.4 MB (9360268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f1a7d478f8c7670b3917c6c5518713e8b3639b3bc7bded3a99a5543c1f63fe`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.9 KB (1940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e39ab211e123a59eca138ecb7270eb494cf5fcd3a62952bbb56475be5c1b747`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced6934e21457558d4cc707f30d7e4a0fe02679a0cb4318e0290f20f32d95942`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bd6d132abe90d38c813e09d681d04097ef025ecb6a1da311c882bb7db84ea`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
