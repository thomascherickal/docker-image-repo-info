## `mongo:5-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:d1caed89471e9df3018cd005da952a880e4cb1fdc66dee9c41cb80bdf3bf737c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `mongo:5-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull mongo@sha256:ee686064aafab7ce028954d421be32674d114a612db3afd4ff04eb4370404ca5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2534589841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950ef6c8eac33725e01afe422ab589b2a04ab266b8305f8cc81558ad41c18a70`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 12:34:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 27 Apr 2022 00:15:10 GMT
ENV MONGO_VERSION=5.0.8
# Wed, 27 Apr 2022 00:15:11 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.8-signed.msi
# Wed, 27 Apr 2022 00:15:12 GMT
ENV MONGO_DOWNLOAD_SHA256=bb8d6bf77df675ef3c89eeded536fc9dcc454f462ef728da53efee7a2c9eb80f
# Wed, 27 Apr 2022 00:16:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 27 Apr 2022 00:16:52 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 27 Apr 2022 00:16:53 GMT
EXPOSE 27017
# Wed, 27 Apr 2022 00:16:55 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2a5d28823cc7f2a78cb6b52a2cadb350e978705d7634adbcfbc4bd80d4637c2`  
		Last Modified: Wed, 13 Apr 2022 14:11:56 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b76d93eb659e63e3e48b6d9371b8a03166bb94560255c6c4aa2dfb0882866eb`  
		Last Modified: Wed, 27 Apr 2022 00:25:43 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb77312d12dd5e9fb7d434a07b0ab3d8a5e0187e7f5728be35307b9ff98754a`  
		Last Modified: Wed, 27 Apr 2022 00:25:42 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd7903123bd6e904ee752e46f1e2116b74c7c6cde14faa1449c5095b621125b`  
		Last Modified: Wed, 27 Apr 2022 00:25:40 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acfa50218af3f7160a5ac62e63ef63ed29fdbbab15aa07a6b9c780488fe1f01`  
		Last Modified: Wed, 27 Apr 2022 00:31:09 GMT  
		Size: 307.6 MB (307625056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c79d66efa39b4ad30679c62a6464e8b909802d5b8b945c9bb127b53a9a5a65`  
		Last Modified: Wed, 27 Apr 2022 00:25:40 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4997d84a0f77ab53a76e25d45072ef19bbd760a35ac5102b076f524488517163`  
		Last Modified: Wed, 27 Apr 2022 00:25:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24567a00eea1debc450b2a0f4ff0c44656e4e5fa5af466a34c1c71db9cbbc375`  
		Last Modified: Wed, 27 Apr 2022 00:25:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
