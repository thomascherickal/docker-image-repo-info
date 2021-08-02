## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:a9dd3bec26866787cd33035a57d380c31c2f13a9b85f2d6d34a1b8bc79f3f9ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:4d913e48d6a0ea2ed11c62cc9fff622727736be864fa3a7fe0f15c35fc4b7b6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274947967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff8abf4d3ed2a1c41241ff4223442903b563fe0a6d8be426bcaed438d42bbbf`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:24 GMT
ENV NATS_SERVER=2.3.3
# Mon, 02 Aug 2021 21:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.3/nats-server-v2.3.3-windows-amd64.zip
# Mon, 02 Aug 2021 21:17:28 GMT
ENV NATS_SERVER_SHASUM=dd14c9c104adb657de4a67a17bdf2fc7d7f55860e7a17ce0c6b9c117d9a50dde
# Mon, 02 Aug 2021 21:18:41 GMT
RUN Set-PSDebug -Trace 2
# Mon, 02 Aug 2021 21:20:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 02 Aug 2021 21:20:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:20:33 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:20:36 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:20:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278db267454aa76e00b506fdd53726da5583419a7844eaa96889ff07827a02b7`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb231d65d7756b89dfbb667d5b24a7bf72ba86e6d5d9c111ab0d08e3e862dfeb`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa0b0c97c4ebf872cafc434ce68ec59df2a3cc66e12e83e929b2d7264559729`  
		Last Modified: Mon, 02 Aug 2021 21:21:55 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe01d11f12da0e487e1ccf3918b3f6a77405b4992df67bc7a092380599cb022`  
		Last Modified: Mon, 02 Aug 2021 21:21:56 GMT  
		Size: 364.5 KB (364483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4bfe4915750d7b0192abb4ef4e16913fc4d8746d369529feaead5f8ef2918`  
		Last Modified: Mon, 02 Aug 2021 21:21:59 GMT  
		Size: 4.9 MB (4938295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd26f2047cfc6ccce7d850ea9ec880c9890f783dd0fa4ea9102c561cfa2aa5b5`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9a1c92d84c4bec202df1e1353e7ecaad58b85a2a2940a9297d14d4548d9e53`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda461d40f36bee8ad537d4225843e28f90f20e81aa8a552d3ada4ef4dbc9f7a`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bf964afbf31f7d4891dc65a1db75f1254d540945a2697c483cdb0375c9b825`  
		Last Modified: Mon, 02 Aug 2021 21:21:53 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
