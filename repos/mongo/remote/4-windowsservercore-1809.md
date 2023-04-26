## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:29791ea0adedb3c66dfd0ebc3b93a947622ae752aa34da1e7b538276da538f81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull mongo@sha256:6e976c69fe46c5331a190f7f109e90088cac67974e5ac0d6f9769ed79eda6499
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2317562904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:240301db3b5d74cd50719d4d6aba7446f3f6fbe8d61b5dbeb72ceb871b4f9b1c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 26 Apr 2023 20:22:45 GMT
ENV MONGO_VERSION=4.4.21
# Wed, 26 Apr 2023 20:22:46 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.21-signed.msi
# Wed, 26 Apr 2023 20:22:47 GMT
ENV MONGO_DOWNLOAD_SHA256=98fc7f0d7942752cdd4bf1eca9f58ed916df6c3cfc4b92fef45616fbc6e667fd
# Wed, 26 Apr 2023 20:24:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 26 Apr 2023 20:24:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 26 Apr 2023 20:24:49 GMT
EXPOSE 27017
# Wed, 26 Apr 2023 20:24:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8421fd8a1642f50929e478c5b576b650506d3d80ad7c39deffe42d7c58a6337f`  
		Last Modified: Wed, 26 Apr 2023 20:33:24 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8719b79456ff559686f6a8b1ea8e538f9125c2f51827c8899f0c6f3f0c2cb58`  
		Last Modified: Wed, 26 Apr 2023 20:33:24 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7467c5108aad82d4a0054deb836fdcd3bb8c117e0739285862e0e4cd29470d2a`  
		Last Modified: Wed, 26 Apr 2023 20:33:22 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05c5042c577426f37c5eca1f7d2d9a46caddbdadf804f0227b72a7b44b2e4ea`  
		Last Modified: Wed, 26 Apr 2023 20:34:04 GMT  
		Size: 246.3 MB (246261885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5766e221e502006dfc410c138ace3d4abc73d62198db0de92e8179373c2fc40`  
		Last Modified: Wed, 26 Apr 2023 20:33:22 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b83887e3bddf2dd3d626b302f6911ff48ca5d7db6f7ad4e6330a4febb6efa4f`  
		Last Modified: Wed, 26 Apr 2023 20:33:22 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7327dc2f853e33af8285dadb5f225bc2400059ca3ed3396c4ea6844e5f9b6cd9`  
		Last Modified: Wed, 26 Apr 2023 20:33:22 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
