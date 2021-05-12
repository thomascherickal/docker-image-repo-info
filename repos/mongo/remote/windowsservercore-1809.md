## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:8917c43037c70887cbb4140acc128cea9c1c2fd7fcb70257d20145baedbd6fab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:a97ab97bd70b4ee260d47bfad657aa45d6d97b0b14c1632b494549c08e840dde
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2710979169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38f334cc67f058217a282d4639a6c8d216cb3276986468d85f2447ac2df4234`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 00:28:38 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 12 May 2021 00:28:40 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 12 May 2021 00:28:42 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 12 May 2021 00:32:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 May 2021 00:32:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 May 2021 00:32:39 GMT
EXPOSE 27017
# Wed, 12 May 2021 00:32:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b76ca32b3a0935667ce199da9cf3dc8f49a43bd76cfa2fc0420c3d4b97e330`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fd08dd311d0b464bf40cfcab2d9a98fab0eecdb07abb54b51d05fd6e1be88a`  
		Last Modified: Wed, 12 May 2021 00:53:26 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003b15d88d3feea95e3452e7fbc9a500e1463e27d7437c2e3c71cc8374a37906`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a096d3e60e3713a8649d486f7d8565f6ef572df05a14cab35cc7eba1a962a`  
		Last Modified: Wed, 12 May 2021 00:54:14 GMT  
		Size: 236.5 MB (236480398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aeb4d7a3233ce26581dc04481318468cdf1d84841cba5ff386130c718e3560`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254dbf0c39fcad87517dcd37a6524541898a6f5f315f3d4e883a468355dcaa30`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430204dde0cbe63c7b8e08baca8bb8b0467cc8380ee15e1c627f49275fe2d3e`  
		Last Modified: Wed, 12 May 2021 00:53:24 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
