## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:4e912b79015d0859d5b6c675d055f80bd7628c8e368d96466b6ab6d9c7a51f7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:ea5bd03ca8c905a9bb8df9bcefe1c70aada9fce64c82d90932dfaf570332087a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691339003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce14639524af68868fed35dda40295ffe16c35eb58b5038f43989d7d60f7059d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:14:04 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:14:05 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:14:06 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:15:08 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:16:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:16:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:34 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:34 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c32056c4535002b64e42d1424edb3a7ac778c308d2d9109f33d738d59c85454`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb115761571c4ba7b8b719d8ee1587c8898f7e13246d1a92ee2283c0f929a1b1`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd93d02cef774a55aa7c6f566b3b5718436cbdae64582cc888ef3b1efe452735`  
		Last Modified: Fri, 10 Sep 2021 00:20:01 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f28336574033153776b7149c4d079b46a95608a291563bc581fc8b029d9399c`  
		Last Modified: Fri, 10 Sep 2021 00:20:02 GMT  
		Size: 372.4 KB (372418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcce3c7fbad71cacb4533bac881f55d312123c387549ca7840f402aa108fb59d`  
		Last Modified: Fri, 10 Sep 2021 00:20:05 GMT  
		Size: 5.0 MB (4955556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d387c2eda58f8b5f8c3889645ec5e1a977b681cb17de77c04de1c643341b18`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f70bbbc8ecda378ae0099ea8e49350ba7d78be681cd5defc71e6f624abca5d7`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b0025f319f789e7c26483abcf5ca7944dc5a1f0a071023d2415526aa310d40`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ff7344cf8ed7957719594d8f9fe4d78b0ef7acc3755bb1962febcf166ac4ce`  
		Last Modified: Fri, 10 Sep 2021 00:19:59 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
