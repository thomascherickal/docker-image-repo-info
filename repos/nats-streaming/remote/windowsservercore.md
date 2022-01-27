## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:5e1d484c7dca916135015dfaec2921b8ddae1a111550e94db3abfc74cb1611a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2458; amd64
	-	windows version 10.0.14393.4889; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:0ddcc2c84f7561dd757922a915f8b895a3642840b77ac65da07ca6ff150b6ed8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721469500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29c41dab84bb2b1242f41f98b1b1114ba6c5317de03592db240813f7c55ac83d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Mon, 24 Jan 2022 23:18:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 26 Jan 2022 01:15:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 21:06:42 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Wed, 26 Jan 2022 21:06:43 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Wed, 26 Jan 2022 21:06:44 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Wed, 26 Jan 2022 21:07:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 26 Jan 2022 21:09:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 26 Jan 2022 21:09:45 GMT
EXPOSE 4222 8222
# Wed, 26 Jan 2022 21:09:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 26 Jan 2022 21:09:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1e63a09e013659f9cb51a44694cf1487fd0ea2ae5528ca387357386508f2b93c`  
		Last Modified: Tue, 25 Jan 2022 00:07:22 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d2d5bbe3c541fe8decf0e3c04bd30aaa74313119e1269d9b03d461638babbd`  
		Last Modified: Wed, 26 Jan 2022 01:19:16 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c644bfc51db2e9bf61379bc3d9a3001f6153015547fefd0af00c693b909146`  
		Last Modified: Wed, 26 Jan 2022 21:13:33 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2796048c785f676d7b62a0263d4631e666d3bd3649c2877b9a2b4bd870ee6b4b`  
		Last Modified: Wed, 26 Jan 2022 21:13:32 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae657cb8a6329c8b06fe2ef8301458731715aa6982e8ef372715cee787eacfa`  
		Last Modified: Wed, 26 Jan 2022 21:13:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e87630bfa7a9f5f7d7bc99bf906aa21fcd20b349b794b23db928320880585d0`  
		Last Modified: Wed, 26 Jan 2022 21:13:31 GMT  
		Size: 368.7 KB (368723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e53af9db8b6cfbdd9b0d02ffa03cfcea13846006c9bf11582639274234b87c2`  
		Last Modified: Wed, 26 Jan 2022 21:13:33 GMT  
		Size: 7.8 MB (7767883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba22b1c14510da1560549ae14e6951c37bed357678330f5866a210226903cba`  
		Last Modified: Wed, 26 Jan 2022 21:13:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c88e435b0f32d1b53b3d86570d47a3b556523b589366f43ffbce400ac311ac`  
		Last Modified: Wed, 26 Jan 2022 21:13:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9428dc8ecce1cf47a8f3bef44bdfdbcba10a0aef7d0d908c808695ff33040dd6`  
		Last Modified: Wed, 26 Jan 2022 21:13:30 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4889; amd64

```console
$ docker pull nats-streaming@sha256:cd7b07b73fc9efec05eafffc4b07507e401f791c341f4fcace5d690f42f5cf1c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290105649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1393fa4d391ed72a261fd64f2320fb2b20badd668be88a3eb75012ad0fc83894`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 16 Jan 2022 17:26:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 26 Jan 2022 21:10:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 26 Jan 2022 21:10:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 21:10:11 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Wed, 26 Jan 2022 21:10:12 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Wed, 26 Jan 2022 21:10:13 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Wed, 26 Jan 2022 21:11:05 GMT
RUN Set-PSDebug -Trace 2
# Wed, 26 Jan 2022 21:12:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 26 Jan 2022 21:12:50 GMT
EXPOSE 4222 8222
# Wed, 26 Jan 2022 21:12:51 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 26 Jan 2022 21:12:53 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:632aaeb77a49daa93237d42e634f5d4574b96f1dafbdbe1e066e9d1341211c49`  
		Size: 2.2 GB (2207519242 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b47e699a2790cbc275f200c0c1a61dc6994f555cabd7b6ee21863e048262d5df`  
		Last Modified: Wed, 26 Jan 2022 21:14:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d7cbf07816862ecf36ecd20ea58c979021c43e241e73299bff9e31a359efb8`  
		Last Modified: Wed, 26 Jan 2022 21:14:04 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8279ff81ac7ee6c145eef09c5b187c80753db8fcb3ebf9cc199f529e1fd9699b`  
		Last Modified: Wed, 26 Jan 2022 21:14:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1e9f1b4cfb6ba011dddcc6a477e7e61ca8a924ebc939e5ada0b4debf05dc64`  
		Last Modified: Wed, 26 Jan 2022 21:14:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2669423d43971fc27cea3ac3f33862032c4cc32af78ddfc7001cd254f8c182`  
		Last Modified: Wed, 26 Jan 2022 21:14:03 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7a79d8d3cb3a08b092a627d208663bbe7369ccc55f577cc5aa9f662c910bcf`  
		Last Modified: Wed, 26 Jan 2022 21:14:01 GMT  
		Size: 329.7 KB (329713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4cdad1539706619f8c6398f2df1549627b88854e6f8be67679b5c86aa19d0`  
		Last Modified: Wed, 26 Jan 2022 21:14:05 GMT  
		Size: 12.3 MB (12259835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026f21fcb46a2ab9a4d2f590db61d059b6f7c29f13caa8af5d3edb46c1593474`  
		Last Modified: Wed, 26 Jan 2022 21:14:00 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07acd3ddfa7dc527e74477f2273aa8cc894653a6679d63501dbac37f6a1d3f7a`  
		Last Modified: Wed, 26 Jan 2022 21:14:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f30e90f702e8671a3fc980a4262e5a9eeba83b071fd1cef806804607b13dcfb`  
		Last Modified: Wed, 26 Jan 2022 21:14:01 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
