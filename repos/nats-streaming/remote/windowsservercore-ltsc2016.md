## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:62945f3e51902319046e2bd0464be26fc730aea2850268b77ce48818ad493d09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull nats-streaming@sha256:2209b5c3482a96a3dae3e8ade7aae5ec6caa7e077ad472779bada808eecbc268
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6287324539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b52052c1bd51b6280c83afbc804f342150ad5265b218136f8b7fb1b464b7810`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 01:55:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 04:34:51 GMT
ENV NATS_DOCKERIZED=1
# Sat, 18 Dec 2021 08:02:56 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 18 Dec 2021 08:02:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 18 Dec 2021 08:02:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 18 Dec 2021 08:03:46 GMT
RUN Set-PSDebug -Trace 2
# Sat, 18 Dec 2021 08:05:31 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 18 Dec 2021 08:05:32 GMT
EXPOSE 4222 8222
# Sat, 18 Dec 2021 08:05:33 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 18 Dec 2021 08:05:34 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6bffd19db3f71ba2031bea25a529c67034869e7e1bbf9e2431d5ee747bd6d6d`  
		Last Modified: Sat, 18 Dec 2021 04:00:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05006360e7d5d5f0fc5160410fd98cfab768e620dca3f3fbc5b44e611e3039b4`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79673abbfda8355eb19c36d4a838ea039890c3b36baaa24cd9c6f350f9dbaf6`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56135df6f0d37ae5054fdc25bf5318d041b879e122c85613d52e71729262aea1`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec44dadd27b2b6ed2c809e4535ad5c1cb2ced6a10857849e9434b533cdb27ce`  
		Last Modified: Sat, 18 Dec 2021 08:06:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f0a80a8e8d81c759bbe086bda6032ced235dd3acd963be9eb97a6aa4fe794d`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 328.3 KB (328284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6eb7f28bcbbc325f606ce67eb09e5996052f69f474b1460ee1a08fd6f326a`  
		Last Modified: Sat, 18 Dec 2021 08:06:58 GMT  
		Size: 12.3 MB (12270678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1b9cee769ed5bc39fd057d6669bc9630960eebf6507cd19a5f4b9ebc5a4953`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df8e108c24c7aff3a16b44fbf9243d457b7d5d45e701f2af5601985424595b7`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298ef1dbe7d3eca580edccaab1932ba55fc39eeef55cb80c3221a4abf9e1f0e5`  
		Last Modified: Sat, 18 Dec 2021 08:06:55 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
