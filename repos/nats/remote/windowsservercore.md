## `nats:windowsservercore`

```console
$ docker pull nats@sha256:c892e8d423eb9100e66d518f443dc34c909d61cbb9ddf3e915d1b2b01ebe751e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:5571861cd5b0f6018aa7855af4e2404c0ce18c6c84998469f37d20ff2b3c1904
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779175732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:531ff1eed7b103984ec29d81ea6f77943f8d3a711b1f4a6369022382a699d410`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Wed, 02 Nov 2022 00:15:11 GMT
ENV NATS_SERVER=2.9.5
# Wed, 02 Nov 2022 00:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.5/nats-server-v2.9.5-windows-amd64.zip
# Wed, 02 Nov 2022 00:15:17 GMT
ENV NATS_SERVER_SHASUM=86c963d3780234e6fecdaf72b9c89c9ecc2fc534d21c8e3ae855d0c062e41842
# Wed, 02 Nov 2022 00:16:49 GMT
RUN Set-PSDebug -Trace 2
# Wed, 02 Nov 2022 00:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 02 Nov 2022 00:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 02 Nov 2022 00:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 02 Nov 2022 00:18:49 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 02 Nov 2022 00:18:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008b3979e40adbc80493c35e40a541ee0cd9f8cfb0d21f0dbb615b61a5800f3c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04f2cde91cfc04742cc431a646b0a0497d5cb0ac69c47f4530a16661f2eaca7`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf94dd1d2f43db680e22d0f214cd977185845f10df9bc06e7482c0eb43fb738`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a68e7f32692839720ce6bc41b42930a1fb73553533f3126fda5f90e7aacf45c`  
		Last Modified: Wed, 02 Nov 2022 00:19:43 GMT  
		Size: 358.3 KB (358324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db97038ec690106eede5d444866ae33a36d942485fd573db39c19207af3241e5`  
		Last Modified: Wed, 02 Nov 2022 00:19:42 GMT  
		Size: 5.3 MB (5305782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f237153f81ef2cffd83842993b4adbfa6bd1bc6e93f4775bef663d5564b28b8`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 2.0 KB (2000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0660057acb9a90d1ec48107439058b6de0b482644e12a14859cda3f5db0fee4a`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d596407afbadde38cf9b8f7a01869e6a2df90f9db2bfc93a669b60b263856927`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a537a0f8dced04ed22fcf2ceade81c6a0f2e2c1e31a8ece5416bb3673b5b7e9`  
		Last Modified: Wed, 02 Nov 2022 00:19:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
