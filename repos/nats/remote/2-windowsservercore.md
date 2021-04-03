## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:91810bbcbf606b0cf379000443d302c7b5d928cc7309c63da19917ca3ff0525f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:79eefa8948e2758f0659fb934899c37b05b67eb96c38b0e8c67c1a0974992423
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480294595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3875d7d95dfdb0356da902eee6142a19a85e38ae7ddde3bbf34b06e18765ecd7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:15:14 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:15:17 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:15:50 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:17:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:17:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:17:07 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:17:08 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:17:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb0ea2b178ae862896fca7bda0c5c677fd82870ca007ebe695e42f058831af`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c9d68c9aa9d29abd0c09f2016e9fcfc53bd185a7403989cec09108f661a977`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b05ed1fd68964dcfc103f5452b7ee8528749d538e395dd36d17158cab031fdf`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3994ed7efdb8fb7c71541583ff656c6c8e54e722284ec414d3ef00145cb43efa`  
		Last Modified: Sat, 03 Apr 2021 01:22:09 GMT  
		Size: 5.1 MB (5064967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c3e4f395cd1bacff8cb6c6a451cfe4d56b4a054cfc15dd1a8b04a9e56240fa`  
		Last Modified: Sat, 03 Apr 2021 01:22:03 GMT  
		Size: 13.7 MB (13681925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc88971a96126558018ca2f17f084db054369de555c8cb84a508c7a1394236e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fa36b1a5dd3f83c94c4e1597659532cb557cd8f9cd414bb81f1049f39924af`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4147b1dd2e59f8f133ab83ace94bf75ef78c0f9f261d49d65b7cc0b84d49438e`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b9455ff088b797d1cff54432e7f275092555cd8485bbf6b4aa926b88077f94`  
		Last Modified: Sat, 03 Apr 2021 01:22:00 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:ea694b06746523df91b7d824d0fc9030b282cc666bf34e937103b72b280d8a09
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817027558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:265f2ee0b7a998cc6ce663873648377be2b81226575d11ed5d1537b35a4118bf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Sat, 03 Apr 2021 01:17:41 GMT
ENV NATS_SERVER=2.2.1
# Sat, 03 Apr 2021 01:17:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.1/nats-server-v2.2.1-windows-amd64.zip
# Sat, 03 Apr 2021 01:17:43 GMT
ENV GIT_DOWNLOAD_SHA256=1f0d48a7ba9200e2572016a9f3e1ec7e630f0518cc0b40950c14ff3a5d900924
# Sat, 03 Apr 2021 01:19:05 GMT
RUN Set-PSDebug -Trace 2
# Sat, 03 Apr 2021 01:21:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 03 Apr 2021 01:21:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 03 Apr 2021 01:21:12 GMT
EXPOSE 4222 6222 8222
# Sat, 03 Apr 2021 01:21:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 03 Apr 2021 01:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf068626801ee0e0c0bd2b1a1f9e05e2d16d27757653ade2a5cc0d971764f50`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e3dd9e9e868f213575a6d17e3fda275a2d47d15e2f9d13ad6d206a0f8567a7`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657647c528aa33d6da248e5aeeb7babe0f7976361e1654d5920cdb0b6c4848b9`  
		Last Modified: Sat, 03 Apr 2021 01:22:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389f475c113034c3ad6f5619cf1bc1b11fdad81b5e5e009ba573539909b23423`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 5.7 MB (5656062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7a05da95e65b18383e1ae5b037f3b75a628a6af2949313789b364e70c3e7dc`  
		Last Modified: Sat, 03 Apr 2021 01:22:48 GMT  
		Size: 14.4 MB (14447531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d02d4cabb443df53f1d6f7a6f93f8f9dda642d034916077f4fab20c5632675`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 2.0 KB (1974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b93a0d4c513ec838b27546bad996f092605e9c8399ad016f78b8b4cb96a900`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8317ff85679d749fdf54c66f1b278c9f16aa11a116c5c0d288bc4f8debe41262`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8b1e736261cff8c3afa409fd73d85b78d6610a610e3b8eb3412798d3a18348`  
		Last Modified: Sat, 03 Apr 2021 01:22:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
