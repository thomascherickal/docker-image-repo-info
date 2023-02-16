## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:48d79159a0a0c4fb52a5f1889f33996e2dfa4b994439447ba39bf6a4c162145b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `mongo:windowsservercore` - windows version 10.0.20348.1547; amd64

```console
$ docker pull mongo@sha256:eac6642804a8eae84bb7f793cb31ca072aee7cf044d61e2702e2c5bb464eee7a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2193062001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea33a650180d9361d5037f530397f3e2350a1df8153d0ba972ec82092ab82caf`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Thu, 16 Feb 2023 00:38:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Feb 2023 00:38:10 GMT
ENV MONGO_VERSION=6.0.4
# Thu, 16 Feb 2023 00:38:11 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-6.0.4-signed.msi
# Thu, 16 Feb 2023 00:38:12 GMT
ENV MONGO_DOWNLOAD_SHA256=935bd3812047391e4295970538d8b33ddbe088676d5356283678368fb1b2377d
# Thu, 16 Feb 2023 00:41:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:41:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Feb 2023 00:41:33 GMT
EXPOSE 27017
# Thu, 16 Feb 2023 00:41:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028996d5eeb6d70e4f35b4acb3bafeee3f326bb40438911de597cad432ffdbc1`  
		Last Modified: Thu, 16 Feb 2023 01:35:55 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e726bd5e1f613004391b7d41e49bea4011c3a223666caa08a0220f4e0fa68d7c`  
		Last Modified: Thu, 16 Feb 2023 01:35:55 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be2181ce4ffdd1925df0debf928317ad7a4380a7bb74cdaa6de05de23030624`  
		Last Modified: Thu, 16 Feb 2023 01:35:55 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f016f7eb5d8c86b2cc5b836b3294c4c423f25ce3693d94d3d76df59229291a`  
		Last Modified: Thu, 16 Feb 2023 01:35:53 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6384495140e8263892737ad41081cf5c4d6b439408aa7c414f100e4c03294058`  
		Last Modified: Thu, 16 Feb 2023 01:37:14 GMT  
		Size: 513.7 MB (513706543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fe62f77f2ddbdcaf5a6fead2ba3c0e821f1cc26e5b17cf383beda8fa5090c4`  
		Last Modified: Thu, 16 Feb 2023 01:35:53 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5708a4f8adb24613d6412881ae7f84f33aeca94782ea1731dc6b06190926e40`  
		Last Modified: Thu, 16 Feb 2023 01:35:53 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00dd8612fcad1f052bb798cc26d8f04858b6c6a56e8f74badee3660324d7fcc6`  
		Last Modified: Thu, 16 Feb 2023 01:35:53 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.17763.4010; amd64

```console
$ docker pull mongo@sha256:e72a981259127b4405a9251952ebfac14de67d1d9263a6cf9f4f157251783990
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2476492237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11511e4af99bd1ab626c6aa85b02b21bed181d6160b510c312b41a9a10f633ca`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Thu, 16 Feb 2023 00:42:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Feb 2023 00:42:03 GMT
ENV MONGO_VERSION=6.0.4
# Thu, 16 Feb 2023 00:42:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-6.0.4-signed.msi
# Thu, 16 Feb 2023 00:42:05 GMT
ENV MONGO_DOWNLOAD_SHA256=935bd3812047391e4295970538d8b33ddbe088676d5356283678368fb1b2377d
# Thu, 16 Feb 2023 00:46:16 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Feb 2023 00:46:17 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Feb 2023 00:46:18 GMT
EXPOSE 27017
# Thu, 16 Feb 2023 00:46:19 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531f6c3ad9784fc2870ea5ca08c4adccd9318602ed534d822e12b8b658a7b0b6`  
		Last Modified: Thu, 16 Feb 2023 01:37:30 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f090b1b4a006448d110a8b6d34deccbea137b29ba3871ec025cf7368ab7abc64`  
		Last Modified: Thu, 16 Feb 2023 01:37:29 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741d1fcb42edc55eb04a1d70a5a2ee18c721d3620a7d21d012c65640ea0b90c1`  
		Last Modified: Thu, 16 Feb 2023 01:37:29 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da4c64cafdbc33a10171ad45cfb037d546eebfc3112d3b38fe5a339ad896454`  
		Last Modified: Thu, 16 Feb 2023 01:37:27 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408bae7c6b4a552369108cf8d91d3c5cafd307f4932de2614ba22e187d564e16`  
		Last Modified: Thu, 16 Feb 2023 01:38:50 GMT  
		Size: 513.5 MB (513525195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0756456fff9609e27ca03b68d128507edd994a79365773c7431d245128cb0a`  
		Last Modified: Thu, 16 Feb 2023 01:37:27 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885900cc33276ed65cdef25e7ef2c7cce32ea28bc4080c6deecbb085457b922b`  
		Last Modified: Thu, 16 Feb 2023 01:37:27 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2da8f21d4d179c9fec9cbe867b979ad7e0e96a6e9951364cb0abc9798e9f89`  
		Last Modified: Thu, 16 Feb 2023 01:37:27 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
