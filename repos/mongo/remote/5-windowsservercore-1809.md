## `mongo:5-windowsservercore-1809`

```console
$ docker pull mongo@sha256:443a371e508f69c67989cde1ba5d5614a11eb5bf6f5f62805ea07553bbe805d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `mongo:5-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull mongo@sha256:8ea82a284b08ed42448ddff58b08fb3e288e57b9a28d9fa5be3459d4b7a8deba
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2345505250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dedf64f5acbc082e15cd708ea6022569db5d7762cfea35cbe9897fd89d1833e9`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 26 Oct 2023 23:25:28 GMT
ENV MONGO_VERSION=5.0.22
# Thu, 26 Oct 2023 23:25:29 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.22-signed.msi
# Thu, 26 Oct 2023 23:25:29 GMT
ENV MONGO_DOWNLOAD_SHA256=ce6c6b3365e23ffc2245dce2030523ef4440fd154b6965ac5d4e19bc86e86a4d
# Thu, 26 Oct 2023 23:27:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 26 Oct 2023 23:27:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 26 Oct 2023 23:27:32 GMT
EXPOSE 27017
# Thu, 26 Oct 2023 23:27:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317d6b7cb8c3f7553d3d2d86869138cf38ab646031070f4822a47782042968d5`  
		Last Modified: Thu, 26 Oct 2023 23:38:07 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8416a9bb72c7fa114900295cc011040644c950b0cdbeb4a32e595aa27a4a5c79`  
		Last Modified: Thu, 26 Oct 2023 23:38:07 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e969bb37d77014db09aec570442bcf37796bf802e756dd14bc4a035799dce965`  
		Last Modified: Thu, 26 Oct 2023 23:38:05 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9adb5d593eb4162bd86dd958cf8b300a91e647ee2608eb10f83f3c48f14341`  
		Last Modified: Thu, 26 Oct 2023 23:38:51 GMT  
		Size: 313.9 MB (313904910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9300d722038fadd078f4e731a316ae6000dd23725d87a73e75d51a2f029f8b48`  
		Last Modified: Thu, 26 Oct 2023 23:38:05 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c817f0698b4dbb310aaa8a5b3dc81d87e627660d6c649877be700aa8c0cb5f`  
		Last Modified: Thu, 26 Oct 2023 23:38:05 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cf5bb09dfba2a8d71d7f6eaab3a0e66211441ed6578894a8b1a640ff9c97e6`  
		Last Modified: Thu, 26 Oct 2023 23:38:05 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
