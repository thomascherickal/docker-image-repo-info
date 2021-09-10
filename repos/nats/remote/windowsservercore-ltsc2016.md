## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:521575d35d4f87b16aa1482f712733b1273962ba4f75353d07327cfc4e324cee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:7f318bb6bf586d9b74b6b8e8097ffabf3b4d16c43c5b9b2dd62d532713aa0305
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276274196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5716654340a54076fb48e8d797d45b91a2e56551a534fb6d800d7d6c61262257`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:55 GMT
ENV NATS_SERVER=2.5.0
# Fri, 10 Sep 2021 00:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.5.0/nats-server-v2.5.0-windows-amd64.zip
# Fri, 10 Sep 2021 00:16:57 GMT
ENV NATS_SERVER_SHASUM=0eae96ad4555f5060b0b6325ba972566b404cd8930b3168b9c0ffe911d15c5d8
# Fri, 10 Sep 2021 00:17:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 10 Sep 2021 00:19:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 10 Sep 2021 00:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:19:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:19:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786675b79153c67ad039b6b8a55171a8167b2ff8c8186ccb7c5cab0b01f47767`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65445b8a1c334a2efce7d34289af9fa682427cba808180c96ce46f39f765e9b5`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08647f69046830b98e59118ace63049f027ad1786cc2aaad037990a4e7a87344`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50cf5c744e8952689c263dbc9800bbe4a032fb4c8df3c8e5028092bdb2a5c9c`  
		Last Modified: Fri, 10 Sep 2021 00:20:42 GMT  
		Size: 338.0 KB (337964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459c701464a835b4d39cc3183fff454248a3045bb433c26b0430f06e91acf1bb`  
		Last Modified: Fri, 10 Sep 2021 00:20:41 GMT  
		Size: 5.0 MB (4957179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb2fb143896bcefca1d8ad8640f3146b771f5b284f01be2b849a048d9ac9eeb`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.9 KB (1938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9f7d515a8e73d005392fc0bccc42761025b86ab370cffe210a552fe53d1cbe`  
		Last Modified: Fri, 10 Sep 2021 00:20:40 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d68902a6dec2675ab57a60716c10ce8a85e58fe54d7abea307bc340452e882a`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e0389f87abc858cef1a365e6b548d7d7762be571608840bc715ef352c41084`  
		Last Modified: Fri, 10 Sep 2021 00:20:39 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
