## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:806b8bf4edc8956db2e8fe23a961df238868b04a2700820d4fc838407abc255b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull nats-streaming@sha256:92df1036dfd3c72bcf7a142e21e3d1776e8d386bbef43a105bb3def3c9b8aec6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5762657171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:186129d9ce285a35807c00a5899c67f185d62239c091634ec5801f481613bc06`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:26:37 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 21:18:30 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Wed, 14 Oct 2020 21:18:31 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Wed, 14 Oct 2020 21:18:31 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Wed, 14 Oct 2020 21:19:36 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 21:21:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 21:21:35 GMT
EXPOSE 4222 8222
# Wed, 14 Oct 2020 21:21:36 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Oct 2020 21:21:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca8ce1a1e304feeddabd9e49e2e5fad5622924c75d97368a7fda9a6eacf3eb`  
		Last Modified: Wed, 14 Oct 2020 16:31:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686b0a818740f1633b74c2225d6f031cc5715c09a4881a438a13fba93d307f25`  
		Last Modified: Wed, 14 Oct 2020 21:22:44 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d196c7cff012be9e007f86a2631135b35f4244060c069a7b117a74ada9de2fa7`  
		Last Modified: Wed, 14 Oct 2020 21:22:44 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f009c551166c1757f25dd72ee5d85fc490974f9850ba13dc1648a96ccce42e`  
		Last Modified: Wed, 14 Oct 2020 21:22:43 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace6d560181c9b8d74da192fecd5f17ff9c2972464f57308d6ab0a4bb5f028ad`  
		Last Modified: Wed, 14 Oct 2020 21:22:42 GMT  
		Size: 5.4 MB (5425219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f421d0869e3cbe5b8580ee0612ddfc8a9afe94d285d80db4f6659869c583c83`  
		Last Modified: Wed, 14 Oct 2020 21:22:45 GMT  
		Size: 15.9 MB (15871237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d937f908a310fa9b1957cf7d45f93cdfede8f5fb275cdc998d945256ed08d6`  
		Last Modified: Wed, 14 Oct 2020 21:22:41 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f3c49e9d40da03d9a3c60f34aa4e5819584d55c708216829aa3f00d408353f`  
		Last Modified: Wed, 14 Oct 2020 21:22:40 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2088679ebef164efa3ed0b7a7a70064336481303027587ac6bce796c5400bbab`  
		Last Modified: Wed, 14 Oct 2020 21:22:41 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
