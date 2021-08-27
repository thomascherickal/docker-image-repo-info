## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7b1ad12d6c6e44e24975eb80e1111d97db29e82416a00dadd5e14a67bf6c0ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
