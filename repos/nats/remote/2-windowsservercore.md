## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:73f511081ca198af5f5c5d1d5d609bf6cfc5a7d43f01e1c93b4b718eaa7bc1d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:6ed34062ddcdb57863540c220de7d892b2b3152ae6599e25ff1405defc63d9db
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721253627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392c84a5f744aeb82235810dec31fe58510c59683d8530e1727645ae02a45a8f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 04 May 2022 21:14:48 GMT
ENV NATS_SERVER=2.8.2
# Wed, 04 May 2022 21:14:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.2/nats-server-v2.8.2-windows-amd64.zip
# Wed, 04 May 2022 21:14:50 GMT
ENV NATS_SERVER_SHASUM=300b9743afa50e02e4e8d43dc212bfde8a871617bd524829114e19ff680dde11
# Wed, 04 May 2022 21:15:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 04 May 2022 21:17:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 04 May 2022 21:17:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 04 May 2022 21:17:23 GMT
EXPOSE 4222 6222 8222
# Wed, 04 May 2022 21:17:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 04 May 2022 21:17:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bba18134d0cef899134f811c0896e8003b4b03b11726200e2d4f09ff3e350d1`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e1de2ac2611197cf7e3985577bdf089a2330268d7f08ad53a25b42fcf7548b`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130538769de262aeb26e810412f9ee58d5b8c1aeb653929a4607901c92363b93`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1684bc7f189afcbdc72f3a0c8eab43e13bbfbe3e8fb412ac51356098cefaeb9a`  
		Last Modified: Wed, 04 May 2022 21:18:21 GMT  
		Size: 359.4 KB (359393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c4f2e32fa9a2920cfaeae75fe3b7e64312357d7a20b2c5e7347936eef6dc5`  
		Last Modified: Wed, 04 May 2022 21:18:24 GMT  
		Size: 5.0 MB (4960732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18367f87433f56d999dc8c84a381afa2e8d480302ea8c78e9169557cd843606`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279a91eef9f2b4bb4964ed362b6786dc737d38e07cb0266dcbe7441930a27f0`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff9295d7bb66afbef49bab61a76a250ae513e6acdd9a8312b8a153c2cae64c`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce0d33690a32dfd5fb8003a197bdc540ec1d876be17a42ccd82d94634514974`  
		Last Modified: Wed, 04 May 2022 21:18:18 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
