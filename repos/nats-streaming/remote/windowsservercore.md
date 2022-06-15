## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:387e4bc728624184186d070a92a55e856aa2a7c2671d96cab32f349b514fccfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.3046; amd64

```console
$ docker pull nats-streaming@sha256:cb04e6e0f8cb5c0044609cd7613ed913be2cb119140614976185c79afd7c7ef8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2671242741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7a3de4c3d8d1e1d28a8b56d4fbaa3964c1a2d2278444e1b274228c290b525d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 14:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jun 2022 16:55:13 GMT
ENV NATS_DOCKERIZED=1
# Wed, 15 Jun 2022 20:57:39 GMT
ENV NATS_STREAMING_SERVER=0.24.6
# Wed, 15 Jun 2022 20:57:40 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.6/nats-streaming-server-v0.24.6-windows-amd64.zip
# Wed, 15 Jun 2022 20:57:41 GMT
ENV NATS_STREAMING_SERVER_SHASUM=86e1e573706b41a109baf84e93d00cfa7e3f4e47d59068bda18e972a7d3768f4
# Wed, 15 Jun 2022 20:58:43 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jun 2022 21:00:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jun 2022 21:00:46 GMT
EXPOSE 4222 8222
# Wed, 15 Jun 2022 21:00:47 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 15 Jun 2022 21:00:48 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:14def1e29581c5e5d0af7fdf9ff44ed6536e79561eb0f0cdff89e322fb87c423`  
		Last Modified: Wed, 15 Jun 2022 16:18:14 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4520d7ed9563408b1887501297a18f62422d296e51341639869af2207b3209c2`  
		Last Modified: Wed, 15 Jun 2022 16:58:50 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7483e5335862f88aab612386a8d8672d92bfc1225b32d52a2ed148f74d71970`  
		Last Modified: Wed, 15 Jun 2022 21:01:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7c87bc1788e53d27522d4bb2d8f43a8e547617199ba747edd7cda27cdef257`  
		Last Modified: Wed, 15 Jun 2022 21:01:44 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4013161f12b7490432aff41c5e928bbad1d39a8ef8e4fa2b573551808477fb63`  
		Last Modified: Wed, 15 Jun 2022 21:01:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab236b9b12c75c2561aea7e6fb22f0c811c235ee743c2800541e1463e60fe65d`  
		Last Modified: Wed, 15 Jun 2022 21:01:42 GMT  
		Size: 347.0 KB (346970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2460c17f4d5c83a035b2d1cdd0c421cd1849432205761674496d76d37ff39412`  
		Last Modified: Wed, 15 Jun 2022 21:01:50 GMT  
		Size: 7.6 MB (7604498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5e9fed9c04491cb82d6444ec9de5c6618def0f385e2ca3a8f331cde3a1bb1c`  
		Last Modified: Wed, 15 Jun 2022 21:01:42 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8726d99209afe5ca774fbe00825e4c112cfae41c3278d97509d9343dce703473`  
		Last Modified: Wed, 15 Jun 2022 21:01:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93db1912c6cede0a947f4c833180439d48696bce41274a8ac01bc5d82004f1cc`  
		Last Modified: Wed, 15 Jun 2022 21:01:42 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
