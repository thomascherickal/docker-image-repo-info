## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0a360392b4faabc3289e601cbfde43584d571f0fabd8ea711760dba99532db13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:bdb716f867395960020da5d1738ba4bf1880fef7fbc386523af3729059e2bf76
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668399020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679f5b34401ac83f1baff684a794d7d84555b238608f57c4c127a9f7d619027c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:26:38 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:26:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:26:40 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:28:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:28:41 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7b157fcbe53b82633afc538ba4cdeb067ebf7f28177b3a9683c3d1e7ce9d57`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043851a001bdd94df595c6168464bab0f64c1c8f065731d9a59b30050d462ff8`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5688f25c5301f14748dd161d8a9cf3194ee728546e6f21f035099be0882edf92`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918272371828c901e18b12b840dfe6c1deeba7bd1eb395fb4b4b48762ac5bc5`  
		Last Modified: Tue, 09 Feb 2021 20:48:54 GMT  
		Size: 229.1 MB (229122627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15ed306e4ceb60ca3e8f86891d04899daf2311cbfefc61c19f0ad2f88548e9c`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe71f1bf221506fc9466f7ccf5d81c5de5dbcf6762c676aef0758acb9c9f17`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c902c703823609a713c38a9c384a7dd1eeaa35f8d46b6cdd85b21cd13b5ac15f`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
