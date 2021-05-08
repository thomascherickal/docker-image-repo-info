## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:cae511104771f0231d31b8868ae3cac1b8f991bcb60e81b44733236d47525ab4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:a601f0fba4299de34cb17a50c80f7dcdeb4100e139c8df4968d76b3de93cd7b7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814999141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0268ef7189c2659b5c9cf424c2237fab5ad356145b53400f1b936d0f8e6bee81`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:16:20 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:17:30 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:19:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:19:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:19:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:19:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:19:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd73175def227cecab8b1d0daabaed653bf698b3998df811f26df3e7e33b9c2d`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c0d0372510261d94e492fc4b8c34dafc5312b85ed72685a2856304eee289a3`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b90b72277f99d3111385c98ebdb1e34e0515ec30a8d6eed17caef4e21cbcc`  
		Last Modified: Sat, 08 May 2021 01:20:50 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cadf6fcab56a60838248eb1f6b2ac2273141b7a404a2ab9e0c0d89f9f9d94b`  
		Last Modified: Sat, 08 May 2021 01:20:52 GMT  
		Size: 5.7 MB (5653916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2609d85a6e72ac850af35a809109dde27760e08c3f1a1916e1b35b51aa821047`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 14.4 MB (14448135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6c38534554dbb86ddeacf527c41ce516c03d8847dba5b0dc30f1f4d23b51fe`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0791626a30dce3a517c9e41798b4874a9b6419ebde4d059b8abb16c4021e7e`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e367eb9da2f71bab653cf5676c106509a942bd9f2a907f9cca1f447e3e8d6be`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a90a989e400a5782487b7cf7d4ec14cc1593da49ee757bbb502ca5769131c32`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
