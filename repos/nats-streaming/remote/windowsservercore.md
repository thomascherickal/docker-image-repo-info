## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:873f62867ca3ce6469cc8df73a8033cc5950c9fd9d1f9ff698e2837eb114202f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:9dadfac2c2164b2db2f437d280a96d23909f72c4cf54645640144ffab451b1ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694437235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5263b600f73c9897a25a6ad86f6e57e29f9e8b17ce3469d56510db758c6bbf8c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 00:34:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:34:11 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:14:42 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:14:43 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:14:44 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:15:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:17:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:17:19 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55c74bf8af074a49872e1e0411ac5572625083d17cb1100c5cade611deeb92ff`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c196111fa2b96deb4010edf39b6c187a5308e45e859c0a062794c2fb5f3f48e`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be5c409e035db76b6c76c2774e8b8209f20e1834a37862ad68a84c7518b0608`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141803b019a1fc302b56dcb3342baf0756b88480ca4d083ee358589caca2efc9`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dc43e6818218b07cf5b6a72f0a86a81a424c7578e183c8748bc7e03b2784f5`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93af83f772b4d8e59adbfeb537345c8d87986cedc1b34413bd84d701cb7715aa`  
		Last Modified: Fri, 15 Oct 2021 23:21:29 GMT  
		Size: 358.7 KB (358738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250c6ad05f6afb5a141b32358734851a7809aa0b8fe53ecea199340cee0505b`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 7.7 MB (7749250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70abe0499859e7991ff7935e2cd570691e4145343846b3f1916c20e63e83de1b`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeb892ccb21479cd1d2461a9b2d91e8a660bfd99b6196f98cfbb187ca564ac8`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405241735b53c04f1deb99e0d57e4306a7000929fc1417f3b611e7941893ecd4`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats-streaming@sha256:8815df5da56bd4d4c6590ee3694d006ef79370de372711e6d9cc58883dc7eb58
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285418812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fcab03497c9b249c4819f3d431685eb7b5310f184c8173cc4a23fc43794bd6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 00:39:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:39:25 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:50 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:17:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:17:52 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:18:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:20:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:20:42 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:20:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:20:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d3c52a3fe41298469bd9ca8471cd22a349f75bf82b049e968c97dd7cbf538b9`  
		Last Modified: Wed, 13 Oct 2021 00:44:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5e5e67c70d509eb320faa6c55dd5fdc5c5440334d85dd07ea0e919299624b2`  
		Last Modified: Wed, 13 Oct 2021 00:44:15 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ed15de932d9979c2d43b9f3222f1bf63ac1e93c8957e8d111528f4eb10542a`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05220fb197a9cf75d8415d18be45957137cfe4478eaf248f84d7c9d4bbfb8b`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9438d74b0196c77383038699d9a8499be3a062d6b3b9024e49979f93ec5d413`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80833d1dbf80f7fb07f4604ae2e1ff98f6126193d8f1969528e6ac07d099dc5`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 348.4 KB (348369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b865d05ebabc15dffdec813d3c290e511d422ed598bbc88873c082770a3c451`  
		Last Modified: Fri, 15 Oct 2021 23:21:58 GMT  
		Size: 12.3 MB (12292917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a8815ed14c2b91e2a24342e413e5b71803558098b12872ea78541ed0342442`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fe138b6fad8ac92c6b741ae450ccde60b6c4a6f8128dcb6e6459c19a0251bb`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e70c279d1c015efeca65bf0b0a05c18186bbb007b19fab36f0f87f311db5a4`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
