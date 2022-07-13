## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:2185d34a08baa2254fffd6480037c66a2091c564c7c652441d163e7e473602c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:dfae260da4b1b30f0dbe480efc2a7811aa71287765113302c555247a3573c322
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2677363569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af592cb0901893fba48dabeba84c806d1b70791a6751af63a243ee95330b9331`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jul 2022 14:40:53 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:40:54 GMT
ENV NATS_SERVER=2.8.4
# Wed, 13 Jul 2022 14:40:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 13 Jul 2022 14:40:56 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 13 Jul 2022 14:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Jul 2022 14:43:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Jul 2022 14:43:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:11 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:49b5d162039eae4fe1f7d6cc0d4b3be061cabb5d1d89950262e1b010e7ed67bb`  
		Last Modified: Wed, 13 Jul 2022 14:16:59 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a2b176476aa48539273d15d106f9687175e98ae9c9a718eb29874b4890126f`  
		Last Modified: Wed, 13 Jul 2022 14:43:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9ea1caa02772da0597ba779df4ccc227978e1dd60feb4064aa66d118e788`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777f37e586af68c6b7df1d868b3e856fff928314a916dbb1199cd57bf0baa56`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f47e5948a3f7df42d74974a6a5becdfe5e98587748a520668a761351153f7`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81cbc2b52ad93c44ea5782e539d9528b4b8371bcaeefe8d4094d95bc246b50`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 346.8 KB (346783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0d8e174ea86f326ba4fce1dbb8e0a458b0d006989ddcb7d641b8d77ab6131`  
		Last Modified: Wed, 13 Jul 2022 14:43:54 GMT  
		Size: 5.0 MB (4959739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704d324de2c24ce52625e9df560ccb9f70dfa158e83cc7bb84133556ef0c065`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8409bdc3daa3e5113f112cf6bdf585a4eb047a256982287a6b2f531b14c052`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32141d3830a2fab08c09cc3863d9627edac56d0c774016ad84e87b8f98d446ca`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f022b00180c3ed89168447954f3e80c281a7c8a79964a6dbe5f894c2fcfba88`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
