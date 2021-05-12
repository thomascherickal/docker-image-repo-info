## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:450bcbcdd85897b9a7a28a99d34701450223b7b96b39838e95493abd18e77829
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1935; amd64

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

### `nats:2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:a1afdd3ea8f102dcc62a70bfb082588bc4b184becad2469e752c8e126ab6df53
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815946596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b825a3f2e49865904aba44cc6f5a2c8b80c0189b1c372477e32ad2c3545888`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:17 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:44:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:44:19 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:45:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:47:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:47:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:47:51 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:47:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:47:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6646c0a4909dd219ffb3eb6eb3709b768fde40ba969a0416a73716211f2a2ef1`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d117e0e9fd386f6d4c004ecf8c18fe24981e5dcf7396ba7935598c16d63d2e24`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c98fa15ec3d078cc3f3da05a4adc67ef14ad1abad5f9e06af54f26121a1d298`  
		Last Modified: Wed, 12 May 2021 15:49:23 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac43c7bec6bd3c410f67cd8fc3336f2ff913251c6251c48f877908df661c8ab3`  
		Last Modified: Wed, 12 May 2021 15:49:25 GMT  
		Size: 5.7 MB (5705594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af8fbf17e86d247bfd4abf90eca1d1e8682d466716786f01230a300844d893f`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 14.5 MB (14450465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236726b5e955bfd7dd64337c1e1f23a903cfa204639b0a377b13f86297815f66`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231f23209351216b06233ad4059b5a5e3eef3e3f5d38896f2306d69bca7efa56`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64daeb968b2f9ad52152de233e969ab4a7acbd81b939b6d12ce9476c61284b7`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6af4f8b0031c6ff433713d50b0f460a68c589538710d23ff6b592b4b1e575e`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
