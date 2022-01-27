## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:3ba4a0aa37f47528d8518d8f209326ad93867ef3aab9305f9725dbb606bff0fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2458; amd64

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
