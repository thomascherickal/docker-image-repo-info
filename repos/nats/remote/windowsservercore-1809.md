## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:96bb5587358dc2025d7c44fa262b026bd159b99afa0f5c38221e9479230fea63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:583a154f872d502770c0c1990662529b2e3ff025276f4616f8436a9886a5fbe0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779177599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a74ba1b75336fd2776df351c7d5b58a594855ec7a7dd96c019aae0d85abda4`
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
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Fri, 04 Nov 2022 23:43:34 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Fri, 04 Nov 2022 23:44:40 GMT
RUN Set-PSDebug -Trace 2
# Fri, 04 Nov 2022 23:46:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 04 Nov 2022 23:46:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:38 GMT
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
	-	`sha256:3f8f2b42cc55a80066c40803248bcd944b2e9d91b4816cd3ce1d28b443d73f00`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba1db14d0368dc5a8550d542ceb29b2547b7dbed75d58bf1b487ea304f4833`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c39058dc1a861d07eb7c76cea4f1453df1c80785e1cd73a57b1cbe54b539e6`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48988848fc3aac57c4657605637681d89e28c7fb6f4111cce0269c7161baf9db`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 357.9 KB (357949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7043fb33d1c6723cd7d2cd093a39eab66e7d100676ffef06a2bd07a2f6332fbf`  
		Last Modified: Fri, 04 Nov 2022 23:47:26 GMT  
		Size: 5.3 MB (5307986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd5ad15cea0202d17fcc0b2a77ce04a4d6ad74b0b3dcd5163365f9e9bbfa9`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaab41075f644d9851a05a34bc468748e87ee0e266027f90f6b5fd21d6a912ca`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91f95f5391a04697266fedd3f9bfa77d45b13155eea7c56c89a956ae2fecd88`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c5b9e0ee0274c8e0f8c62e405c6ea9629b10afd27bf4663f0eb9be31e996f`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
