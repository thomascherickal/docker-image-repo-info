## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:ca9cf9ebe4d0aa6306e7b53a7a092ccd2f69eeec24646357a0eef697bdb4f647
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:418f75da35917511a99273b446dfdd3b9af8ebe30c5d426238b560732cf34164
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278098651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ff3a0c76070dc9acbd5f90fc2a782f7a6961f87a2133c161ccb245055dab40`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Wed, 13 Oct 2021 00:39:26 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:39:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:39:29 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:40:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:42:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:42:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:42:50 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:42:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:42:52 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:594cc3f90d80a96c00df55188626147f8170f580b7a712a0c1a975dc380810a4`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9c3734400dd553e993f978090779922711884084c6b9a08af8a80c2a4c03d8`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5512210ab9d2dd13dbf25ad44b0abbe94f44ecc69232accf2bb4f33b4374fdb`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c468f554d337e3a687604929a6519c0c88de7093c175ab49843c390c084c48`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 340.2 KB (340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40948c5a62dbd876eb1e51cb91daa60ca1c32b8b38708df7f00db35c72d7ba`  
		Last Modified: Wed, 13 Oct 2021 00:44:17 GMT  
		Size: 5.0 MB (4978594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b76e0e528c691436c7e1006a94cd748a73b32eea4003cef86de73ae3516b30b`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aa08fc51be79a24b847a81556633117e27175161b1f614adaaff26405db431`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.5 KB (1452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570aa2e9cdad8f81f73820da764a7820ed0a28d7100d87f742322ba78d90f05a`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc825431ed33b4460730dbd1909422da70adbffeaa8f8586711474f5780d733e`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
