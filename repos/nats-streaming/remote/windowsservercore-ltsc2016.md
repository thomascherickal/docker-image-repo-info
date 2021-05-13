## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:625ab75dea32121df296345016a44bcaa577d91d7c55b131fb28fd842ab65181
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats-streaming@sha256:d15f6cc0f6f200c03c249c6fa30e1d993feabdba06c9bfb4dd25a41cb75dba02
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817500079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77c238ff37580c7dd07576778ab4a469bb8b538c9e3e9990a2d98c7326094ebd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
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
# Wed, 12 May 2021 20:11:37 GMT
ENV NATS_STREAMING_SERVER=0.21.2
# Wed, 12 May 2021 20:11:38 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.21.2/nats-streaming-server-v0.21.2-windows-amd64.zip
# Wed, 12 May 2021 20:11:39 GMT
ENV GIT_DOWNLOAD_SHA256=5d4367fea29116fcd70c364c8e808d6bc8e74214effbde83dd9548455bd06df2
# Wed, 12 May 2021 20:12:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 20:15:02 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 20:15:03 GMT
EXPOSE 4222 8222
# Wed, 12 May 2021 20:15:04 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:15:05 GMT
CMD ["-m" "8222"]
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
	-	`sha256:7f3010a7dd8667ca84982e9114e1dc65712c28bc68c365842b10a045ca612037`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df06200a155b162a6be73cde9177db0ddf3ab1d3cfbd6cde1716508ea936e815`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e23a0cd6171825cfd2bf6df17479e82e5845162d61bf74cf02daf44b78ba106`  
		Last Modified: Wed, 12 May 2021 20:16:28 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67048fb7884ce62e43c9c94e93c2469620bc4f1c31de0bfed360949a4856b32c`  
		Last Modified: Wed, 12 May 2021 20:16:32 GMT  
		Size: 5.7 MB (5699433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c112a8566705980bcc28d7b657abbc41bebdba6f14cc110792896e37a8ad36c0`  
		Last Modified: Wed, 12 May 2021 20:16:48 GMT  
		Size: 16.0 MB (16012020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61d35a77f28396bd2da2e43c4fdf316968fa5dac4db17f07873ad8f2f778e54`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96acafa52a9f3be44164c214903b7fffc48d9030807ce105a6c09093f4ebe1b9`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b24723ae97946b0dbd5bf2b012548e33ca907518a500ca519e4bb0317bd31e0`  
		Last Modified: Wed, 12 May 2021 20:16:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
