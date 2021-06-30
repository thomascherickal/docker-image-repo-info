## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:93ac3cd4a8b8b007880643270736917965c1417da426af8f293014475ac55768
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:dfc1674cec617d038182099763e8e21ae02caab5b0cbcdf3b294b164cfba144d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646702292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891b94f87075103849e518eb50b76433a17ada32f8d1cf5aa36e530521d6a7ab`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:16:09 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:16:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:16:14 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:16:42 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:17:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:17:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:17:48 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:17:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:17:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c372ca63b1680d65d6a15156585166129bcfbe52e0d05d0054fb79aef686c21`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d56dca1f1579b9ec59f1d6041c16b91b6f68baf0084499e2a85c1405d969db`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e1b684efe630f2971519c8b17b93b91570783e8fbdf7e7ec7f29b55debfca4`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99faa4fc39833933dd9eb1cbf6b84eccc63727e8b32eb4705e1dec20166b5a49`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 363.9 KB (363912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ee24bc113845fef06be0fc93dcd98e34aa2e27e9623df01a966b142e697c5f`  
		Last Modified: Tue, 29 Jun 2021 22:22:25 GMT  
		Size: 4.7 MB (4740124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e272136ec5116ad206285b67f3beb3298d68d6c96273dae139b98b326d71cef`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 2.0 KB (1958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b975b0b42baf2261e7a3ebb135c8b398592c2445b335b404cee3476917b4ab4a`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a43a208d117f790575104759c3ad082ad2d1e74663fe794882536de5c7934d1`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7916c3fd7bebe37b25576dd2b9f6d9b72be1b48773da796349d7ef3058365`  
		Last Modified: Tue, 29 Jun 2021 22:22:20 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
