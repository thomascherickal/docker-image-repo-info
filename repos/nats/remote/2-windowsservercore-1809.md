## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:071e59383a264b91a6f178c3a91ea720ee076bf36d8fd2fc4db799bd1a0ba68b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull nats@sha256:5fecb38d3c0ced714fbbce17d99734bbbdec770aff9ffd6183b6b7a6b3a2d565
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668599436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f806f4bcedb17b412cb3557b657559a2b1a000bd205afcef4f682ff7006e9243`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Wed, 15 Jun 2022 16:55:14 GMT
ENV NATS_SERVER=2.8.4
# Wed, 15 Jun 2022 16:55:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 15 Jun 2022 16:55:16 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 15 Jun 2022 16:56:17 GMT
RUN Set-PSDebug -Trace 2
# Wed, 15 Jun 2022 16:57:51 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 15 Jun 2022 16:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 15 Jun 2022 16:57:53 GMT
EXPOSE 4222 6222 8222
# Wed, 15 Jun 2022 16:57:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 15 Jun 2022 16:57:55 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:cdba438d9f4e6ac809d411de641febad0213e4f10d7bc1a0a1c6cb75fac24f2d`  
		Last Modified: Wed, 15 Jun 2022 16:58:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf63bdfea9b27af7759bc6271c2ac1941f0bbd71f5e303b6cd3d91e95c991e2`  
		Last Modified: Wed, 15 Jun 2022 16:58:48 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a01537b763e3a844892d72c0f728d5faeb0405e48c661a0f80b2f110d3e5947`  
		Last Modified: Wed, 15 Jun 2022 16:58:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f70b3c1991cfb80c1802b2fa4190b0b2ddbae35ec6a7cd088864afdb8003a5`  
		Last Modified: Wed, 15 Jun 2022 16:58:48 GMT  
		Size: 346.3 KB (346348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5de019caf6cf0d5cf6d7f2cbad475401d4fa5d690e40605bb8385371e22fbc`  
		Last Modified: Wed, 15 Jun 2022 16:58:51 GMT  
		Size: 5.0 MB (4959820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199b4cc41e1bbed1641a914a5ed8c58a43a0cb0b2670ee5aff11ccc61c29ca94`  
		Last Modified: Wed, 15 Jun 2022 16:58:45 GMT  
		Size: 2.0 KB (2006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420d01793d06cc01456f58bdc3bf43d06a5df4eb30a9b45c9021611787510412`  
		Last Modified: Wed, 15 Jun 2022 16:58:45 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fe0969c6075b2c6ae912d5c812758405bfe3bd0981aee28c7c97c3ba7e8801`  
		Last Modified: Wed, 15 Jun 2022 16:58:45 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad6241e0853a3feacd918e74c4e4467bef29cf83aad3962ce66f96c5f83037c`  
		Last Modified: Wed, 15 Jun 2022 16:58:45 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
