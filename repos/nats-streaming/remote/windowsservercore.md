## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:08798cf762b1971f7733e42d08e6b035fca00c85df8d6eed35566a9b42fb43e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:f4e06e330b3f5b04a0b4869e1475a1be8dabf7d0c555d31638cf63c2f7ce8e05
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2079954789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:730388aafd3fb6e94a5fbb3ca2923d908a88a70987542cd8f3aec0875aa6e422`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:48:58 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.3/nats-streaming-server-v0.25.3-windows-amd64.zip
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b25aab68b84cba76e3edec5d524d2a792f460127d159ecb4d2e6168c7635c10c
# Wed, 12 Apr 2023 02:51:00 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:54:00 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:54:01 GMT
EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:02 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:04 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d307d893fbeb91714142851c9b77274bd7d8558c0130d095791519f1b00993`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf34831b97e978505e0c96019e7893d245a7ccd9aab9895bb0a58b9ccf33dfca`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dfeeb40c1ca2e0d61377dd9a76d1be12884552db49acaa27b01b952472ba92`  
		Last Modified: Wed, 12 Apr 2023 02:54:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169dda2907fa6bd3400d8e5d242650dcad43a8e7f28d768eaac7d4cf05f35fc2`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 495.5 KB (495517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1b747c5b3dcc333c8277218e668fe8a63909452f67ab1bd68bb5ad00b66a94`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 8.2 MB (8156762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8066f145c6b9d10d87a1e85b0e94fd3b8e70892bd838575c746abf7bce634c`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ff92a44dfc6bd0976cc42f1b4f0eb81db01f740d36ad047e6ca87b4e861842`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68ea5be3292c7ee712b067942f62560398f0d91609a49f72c4bddba19d5879d`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
