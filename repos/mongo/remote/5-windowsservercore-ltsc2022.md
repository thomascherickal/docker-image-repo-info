## `mongo:5-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:8661a8140734c3742d5c730304958b4edf09b575e71f450633dd8196246a04b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `mongo:5-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull mongo@sha256:e79f450c86c20a086b9aa1594a7653306f05a35769d789e8bfececb5b662b18d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2608683566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d4b4374ca34f78c69c71c51fc4a741a5328ce3e2bb2fced97cd4e80737c49b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Wed, 13 Jul 2022 12:42:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 02 Aug 2022 01:15:06 GMT
ENV MONGO_VERSION=5.0.10
# Tue, 02 Aug 2022 01:15:07 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.10-signed.msi
# Tue, 02 Aug 2022 01:15:08 GMT
ENV MONGO_DOWNLOAD_SHA256=5feeaf02c6a1a9125565de2e3e44a6c11d920427db31d2ef3b516e2832dcff9b
# Tue, 02 Aug 2022 01:16:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 02 Aug 2022 01:16:38 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 02 Aug 2022 01:16:39 GMT
EXPOSE 27017
# Tue, 02 Aug 2022 01:16:40 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a596a8bd7e59e41c674f92ccf4bda0ac985c9143ed67987de02e069f2fbf87de`  
		Last Modified: Wed, 13 Jul 2022 14:16:39 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5297ce4fd6403a2af06d378e8e3e89d60aebd10e2d4cec98fea8e646062628cc`  
		Last Modified: Tue, 02 Aug 2022 01:23:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3495e4c8ca64350d36f43862aef3ec47e05193c467f7555572a09b57cdd3e15c`  
		Last Modified: Tue, 02 Aug 2022 01:23:59 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f84569e8efe2189c6eb5b60fda0ea0b305913e4dca4e04a42579060aec0c11`  
		Last Modified: Tue, 02 Aug 2022 01:23:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d49e80acaf280f76167ab3a9b344ecd90c30ee8f20f790134f7fddb8b2e6430`  
		Last Modified: Tue, 02 Aug 2022 01:24:53 GMT  
		Size: 308.4 MB (308442036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4641064fa25c31c49f540c543b3ed82645ddf5fcc09882e1def8a0ef9f347f01`  
		Last Modified: Tue, 02 Aug 2022 01:23:56 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9882fca01e9478bcef9324a7dcf1831c903a5d0a8e46361a3c8af24ac207d4`  
		Last Modified: Tue, 02 Aug 2022 01:23:56 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c5fb1d7173df9bf96adf7e1b5b531251ad43e1607615840621155e3b2288b4`  
		Last Modified: Tue, 02 Aug 2022 01:23:56 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
