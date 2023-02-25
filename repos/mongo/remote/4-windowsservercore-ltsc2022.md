## `mongo:4-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:980fdaf8700901773d3d07827a09237bf6090d56d8b61427c946d52b27251e20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `mongo:4-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull mongo@sha256:45d0e84b330e046f6947e47aeb81464e7af58e0c8b1fe5e39e1f4dbae792515b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1925333848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4817d2d802c6025f43f157aec6b248ec88562c02e3e026dcb504414fe42854f6`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Thu, 16 Feb 2023 00:38:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 25 Feb 2023 00:23:18 GMT
ENV MONGO_VERSION=4.4.19
# Sat, 25 Feb 2023 00:23:19 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.19-signed.msi
# Sat, 25 Feb 2023 00:23:20 GMT
ENV MONGO_DOWNLOAD_SHA256=91e83f2fc3ddd3ab0bb170d26b89d80e4268a563deee6ce72313de5774875f08
# Sat, 25 Feb 2023 00:25:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 25 Feb 2023 00:25:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 25 Feb 2023 00:25:09 GMT
EXPOSE 27017
# Sat, 25 Feb 2023 00:25:09 GMT
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
	-	`sha256:ba43653840a42a2b44a0a578c02d136c353067ec3f3c6f5843ed53e4dbcc8890`  
		Last Modified: Sat, 25 Feb 2023 02:23:25 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6101f31b357fd8aa4f56122741593a133101a622ed7a7d59ef6475b8df72e23`  
		Last Modified: Sat, 25 Feb 2023 02:23:25 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b49c9440a752659808680f5681ea4f31c17f88898a9f9c192998a602df7ec01`  
		Last Modified: Sat, 25 Feb 2023 02:23:23 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36cf08719f0c798091f890393817422398e2cb69f8c879f29d8710fdd950de9`  
		Last Modified: Sat, 25 Feb 2023 02:24:08 GMT  
		Size: 246.0 MB (245977989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e76ecafc93b027bf8bdd384e82111952821bc3c4b05acd1b3c07e84e5fadda`  
		Last Modified: Sat, 25 Feb 2023 02:23:23 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd60b3b8040f2d0e36320a6202faca137031cca892dd72cf7817bc6107a95e8`  
		Last Modified: Sat, 25 Feb 2023 02:23:23 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5996c5532c42d2fed68c7ff806e5ee33cdb625de6c33a830f6df2a9656e3375`  
		Last Modified: Sat, 25 Feb 2023 02:23:23 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
