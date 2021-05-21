## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f5e1a7a908d5beaecc090e7ca32ddf92f1e7b3d646ebf82cc260ba78a1bd27a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:af6a479ac67823cd29228d23d3fe797e8e009e9c1987aebfca481912f7db1bc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815986529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:109f28c28e9f87f8c0f69c42839e0a3f8636808c2e84027981406fc988afbe5d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:43 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:17:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:17:45 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:19:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:21:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:21:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:21:19 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:21:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:21:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f3603b9524e93e5215c2abba5afdf68a7402c199c6044081404215e3ca09ed`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfaee8f415fdf30a7173aca01dd406a0dc11b64bf22445d8ba10838ab73f5cc`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba0596bf5825d8b175760cadb4aa03bc8bfff3cb41088d8bed50f495efc9974`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933b94135b57dbf1dbc2823aae3e8c232d5078c506cc6ab357dd294fb8308187`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 5.7 MB (5699902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b118a826228e68680a9764693342bbf52ffb2c132cd3482c8235c8637efed1`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 14.5 MB (14496050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61cf67042c8c5449c0e8f5baa07aec6e3907808d9c64e79d22e6bafa152b5ab`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67754daf786179eff413898a2d98262cb69b817c93a7659504d2220af5727780`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067668e0d80f3d3321ce3cfdfdb3e4f901ff14219b46fc2d432115e97afc4cf4`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17dc212c86917e270b694d1cd121320509bb1afa338b24c3d2d239dee1c19ad2`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
