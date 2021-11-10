## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:c5b7ed794ed1ea3bc9973244e683bd5dfb902e0bab7882855f15fb1696802bb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats@sha256:ad29bbedb595a4b3fc815bb5013d6af6deb55f459d016ed438c89308084ab2ae
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2711460012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c235da1808d9829823250ce435b177c85ddd1340f0878343bb5e4a1521602a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Wed, 10 Nov 2021 17:00:41 GMT
ENV NATS_SERVER=2.6.4
# Wed, 10 Nov 2021 17:00:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Wed, 10 Nov 2021 17:00:43 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Wed, 10 Nov 2021 17:01:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 17:02:51 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 17:02:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Nov 2021 17:02:53 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Nov 2021 17:02:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Nov 2021 17:02:54 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:46075e93c469fbc556a996840e6ebbd02849d7518dcb4fb9feed459795714e03`  
		Last Modified: Wed, 10 Nov 2021 17:06:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a915f8554b2287a16ae0945b328b1d7d315b85bd0eda548bfde73d7686a79c`  
		Last Modified: Wed, 10 Nov 2021 17:06:11 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160d4eabf66e1adaa7841404639039b5becdbfb43fc726b93da058b0552478b7`  
		Last Modified: Wed, 10 Nov 2021 17:06:11 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f61c483196bb419b4709f89f9df78e12e7f6dab4ad8094a5aee57e021c97eb0`  
		Last Modified: Wed, 10 Nov 2021 17:06:12 GMT  
		Size: 352.3 KB (352252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e167a3b21bfb85235d9775123ea38ca0d4a4c71383ca34a95f3e203f6afddfc9`  
		Last Modified: Wed, 10 Nov 2021 17:06:15 GMT  
		Size: 5.0 MB (4973372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1d94f1b880ea3ea631c3f6e7ddeffdb30d7af80b037e2fdb55db516d018dd5`  
		Last Modified: Wed, 10 Nov 2021 17:06:09 GMT  
		Size: 1.9 KB (1939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb1edd94e1965c70a2bb20e8bac08446704c452ce9342438e89afe2febe9906`  
		Last Modified: Wed, 10 Nov 2021 17:06:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2d4b3e56ee1751a9373a33f5b9d58f1843e22f5ec7cc88f00e6ef369d7d9f7`  
		Last Modified: Wed, 10 Nov 2021 17:06:09 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfe4f9233effe09d6160c4278ac3a375234523f40d18c3a826dd9e741139be8`  
		Last Modified: Wed, 10 Nov 2021 17:06:09 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats@sha256:b8b34e3ddc6569eda34bb1d124a6c427fc3820313fea9618b702a1fe9a281914
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278456953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33c0d6fd779bb5acd23d794cab7a62d0a39d140ff94c890f83cdb2814d63808d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Wed, 10 Nov 2021 17:03:19 GMT
ENV NATS_SERVER=2.6.4
# Wed, 10 Nov 2021 17:03:20 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Wed, 10 Nov 2021 17:03:21 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Wed, 10 Nov 2021 17:04:06 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 17:05:30 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 17:05:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Nov 2021 17:05:32 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Nov 2021 17:05:33 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Nov 2021 17:05:34 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:fd4a229bc6e55d797c98ddd01e4d2dde702cc15dfa57f7822427f4b0c7520a1f`  
		Last Modified: Wed, 10 Nov 2021 17:06:49 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99e43798e75fd46299bad03217fa38c7f0b36023271b5ded075984cbf2df237`  
		Last Modified: Wed, 10 Nov 2021 17:06:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cc0e5c4cac5fdb636f2f1103de5fe3668597d85350d0d91b1834cc44a83b44`  
		Last Modified: Wed, 10 Nov 2021 17:06:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb570dbf36f38785df2fc8983ad0725e443f375bdd45954981931f0137e26ea6`  
		Last Modified: Wed, 10 Nov 2021 17:06:49 GMT  
		Size: 350.2 KB (350227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007ae15590fbd4c2fc97f92a5fd9f4bbee82f5e8d9da82ac218b4d5002f1a50d`  
		Last Modified: Wed, 10 Nov 2021 17:06:52 GMT  
		Size: 5.0 MB (5002607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbf9bfc6a773256d2ac9289665265759ec89a55717d181030cc64c706b5be9a`  
		Last Modified: Wed, 10 Nov 2021 17:06:46 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92c772d8667daf25c2468b4b149536c7e9fe55a5896143d2e4eba0ca861cede`  
		Last Modified: Wed, 10 Nov 2021 17:06:46 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca4dbf235f9fc558316b5e2119a389936545de68e74f1ad4acd18c7282eff43`  
		Last Modified: Wed, 10 Nov 2021 17:06:46 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990cb23cac15d214ca7bac2df486570024c5eb19e214014a88b247c684605ee5`  
		Last Modified: Wed, 10 Nov 2021 17:06:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
