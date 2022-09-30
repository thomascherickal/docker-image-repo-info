## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:3357d7889ebcb10a163ba56eff66f60ff010e161b38e1f401cc136e7a6879baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull nats@sha256:214e04a7dc77ff783ac336d010ba64eb98f2c8722d522260bf340c2df3d521e7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2709236645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cb30cff6676167599e8b4fd9f6b053b3e6fa2f5418a7a419e631956a014e9e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Wed, 14 Sep 2022 13:39:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Sep 2022 15:38:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 30 Sep 2022 00:15:50 GMT
ENV NATS_SERVER=2.9.2
# Fri, 30 Sep 2022 00:15:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.2/nats-server-v2.9.2-windows-amd64.zip
# Fri, 30 Sep 2022 00:15:52 GMT
ENV NATS_SERVER_SHASUM=cd3d2a9d78c235292afc27f812baee7817180fcfe5ebba662e72f0cc821d04fb
# Fri, 30 Sep 2022 00:16:59 GMT
RUN Set-PSDebug -Trace 2
# Fri, 30 Sep 2022 00:18:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 30 Sep 2022 00:18:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 30 Sep 2022 00:18:31 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:18:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 30 Sep 2022 00:18:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c428406510f0a47ed60f28060a7d625d42344a95fdcb7c4f5746fb8857c3328`  
		Last Modified: Wed, 14 Sep 2022 15:42:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4bba85c5cc970a66b01ed6f4cabffa7705a0bdbc18907894f94c09b5ee2618`  
		Last Modified: Wed, 14 Sep 2022 15:42:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29319534b1836908aab29077ce165236693f20e5abbb69a70639c6cce19223b`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34f7b3a98b75cbb6f21f33118a7f43b9efe7d7d8ef5d9f47b5ca73470abd339`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2119397eb3051d4784ced2882a1c0f1d2995cec67f5954fd5f33fde4b6ab4c3a`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdecf001ef7e4a9db54aa1a639bf5036f69cfc71a2d6b1b9089c1a3810373aa`  
		Last Modified: Fri, 30 Sep 2022 00:19:24 GMT  
		Size: 358.1 KB (358089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a5a2ffe352520814f5794422903ec9e717d37294931ca81f856257a419ee1f`  
		Last Modified: Fri, 30 Sep 2022 00:19:23 GMT  
		Size: 5.3 MB (5300456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c11ae75a170747a9206d993fe059c9cda9f34c08c9f2eb90bedaef90f322e`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8020be63ec6ec39f4443bc78e114caf9c24c5686fcf3f84a8c74f38f61b864`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d3d068429b4966cc13e153bdbf220b0259eb72a6a3f507fc5172a963499566`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f588edee9a48a943744711d7d4dea00d9e842180f05a759c2edf3e50ee10e06c`  
		Last Modified: Fri, 30 Sep 2022 00:19:22 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
