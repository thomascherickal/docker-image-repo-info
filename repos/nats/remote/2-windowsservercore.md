## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:95c7b2edb68fffeddc422d8b2a36778e3e589d9df49014991f4a2e9ea47134f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:d7323469b7f3bf803d8db59cce7c9375b0c95627898b7ea51d364561b96ea174
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484222239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce0ce6bf54d9a83dc699dc925cefc4da62be50613ad270dcd2d7cd2aed19e4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:14:10 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:14:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:14:12 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:14:43 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:15:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:15:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:15:57 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:15:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:15:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d6a59546309673d4b20f6b764e6cdb66ef15109c8d058a3a6fafc152a44aad`  
		Last Modified: Sat, 08 May 2021 01:20:14 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c48747fca6c2cf91251deb0b3843f44b8758ebd29ee8fa0edce17b9f7dcfd5`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8193a715c0836417f1d9325ca56cd00c0108132642f3f0f22b98be9449c6b8d`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a6b950b0b7977911f8e95d23bfb1102309fd1c944f92fe940e056088742faa`  
		Last Modified: Sat, 08 May 2021 01:20:15 GMT  
		Size: 5.1 MB (5096312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7da99923a0ffc9f03f1732f727ba585738acaab6860d0187a480de49558c2d9`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 9.4 MB (9358928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a1256dcb38b1bafce26f943536a7dd9a39c7ec54fd4136cc49a3f5ef6d8d6`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab9f770e3ab4e0d968cb65264ae0e9bdd4382b8d3a70deb59617091b2af9a9`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d4f0c5e71e780eacc043bd6bd9aa62cee1de9e6fb4313c2b195a07f88757e5`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89f86179058b328103f74f4216154e7c83ad10dac41222649baf934a5ccacdc`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4350; amd64

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
