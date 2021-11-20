## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:24b7c3eef25b0f52a4eeceefcaada76227c649e3e2ae98e4b3a570d59a8a6dc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:6f64bd15b581a70d6dfe857f3b44772d1757080d32fd1b99a19d8807def213d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714275444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91c386ba25006af61aa18afb0f4ba34e37130c67698f7f702f6b8e73d1d80c71`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 14:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:00:40 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:15:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:15:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:15:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:16:03 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:17:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:17:40 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:17:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db1ba835bccbdc73ef254c175ca6ae0dc3f0bd759c1910c3b123cfb9613223be`  
		Last Modified: Wed, 10 Nov 2021 16:21:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3df59793c391e0eb7e6a2ddb65801dfa94397b370daa52d04e242ba0274e3d`  
		Last Modified: Wed, 10 Nov 2021 17:06:13 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8527719d6ca5920291f35175b6c32f82952164d42b880f25f57e2ab782716f6`  
		Last Modified: Sat, 20 Nov 2021 00:21:14 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5527fe17246c670fd28071726d0070083f7817bf7a283ee290a4a3578be1c529`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa3900f098cee74ded07ca4efb271ae252d7eccb30ab9f2b5a6ebef3b90ffb`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceabfbc5f736cd2fb608eab7684b37557bba10062b0907a5f1cfb3a82eaf527a`  
		Last Modified: Sat, 20 Nov 2021 00:21:12 GMT  
		Size: 368.5 KB (368487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b742456a9e3d889a1da0049b32c41d9d8c0bcfe02c18bc2e5cb8799f0f453c`  
		Last Modified: Sat, 20 Nov 2021 00:21:20 GMT  
		Size: 7.8 MB (7774527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c68e60ff51543de0cd01cacdc9b50197cf509ff41cde3836443fbce7bf83467`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919e7cdd885b3a08ac5cea5bd5ac952f6ba0788a0f0237c536fd480fd5bae9b7`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab6f9a5538b2a14c942766e01516128ae2c95e811132f8101ac366b93f7b6a`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:a8754ad059b322a076af9cec4038bd0105348d25833189928402564118e1d5ea
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281259279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7b89781f458ba786a9ef0842c06ad7b3548e55e6f5d4a0595b002962db220d3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 14:32:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:03:18 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:18:06 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:18:07 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:18:08 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:18:55 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:20:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:20:33 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:20:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:20:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6f303e73635c7923a8c64f8938e7ba4c10210fd15a6ce63aa8a62d5a8ea8c0a`  
		Last Modified: Wed, 10 Nov 2021 16:21:33 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5db4062c12269959ca71caf00b70e9baebf61b90c49c74db0e2cdb04cf83e8`  
		Last Modified: Wed, 10 Nov 2021 17:06:51 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef5340cf4b5229cb811aded6948a78dd070b1dcd7d9c79a163dd4bcdfdf6e1f`  
		Last Modified: Sat, 20 Nov 2021 00:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0992c1fb2bdb48b803b13b4a53e6c0cb2fdd68a80612186a9c860a467f826463`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1f397ce101e6984fb89ec5963b486f147cc90083474ee83e5ebabb5ed34439`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8ce7e3e4df470099c34c35a291bbc11ebee219db5322ff65ab4d19856a864d`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 359.0 KB (359036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed4996f5a535c518a031301e7d66d2f866efa97ec83dde420c909ae39c7bc4a`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 7.8 MB (7798409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfc383e29d1dc876d8581691fc650f37a769e12321b24db3221b4e9243f7a11`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1db010ba3db16a3ebeb3a7ff12851946f6e49c72e22f1082743768ef2e0f9`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a31dde888d46608b0de9acdfd5988c297ccd2b1187c681185687b27b283dfd`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
