## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:914740ba290018418e61411baef80f37831cb3217d0d8fa49cd37779efdc15d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull mongo@sha256:c23c97351d4cd912cd717105e0505182f1ffe03c8fabceb7db956efe78f2154e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6506771623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f12849d50d0016dc820f3597d9429917d21e7577652df1a5cd2f9b3e18970187`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 14:32:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 19:17:38 GMT
ENV MONGO_VERSION=4.4.10
# Wed, 10 Nov 2021 19:17:38 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.10-signed.msi
# Wed, 10 Nov 2021 19:17:39 GMT
ENV MONGO_DOWNLOAD_SHA256=b48fbc7ba392f505a89af03301ed8f3f99b35c6ee8f3c9595cfebacf26ba68ee
# Wed, 10 Nov 2021 19:19:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 19:19:44 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Nov 2021 19:19:45 GMT
EXPOSE 27017
# Wed, 10 Nov 2021 19:19:46 GMT
CMD ["mongod" "--bind_ip_all"]
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
	-	`sha256:a8e8deed4c6d73c4c25af1cd18245985c3ad0588a6e0ddc583c0bfca1e76510c`  
		Last Modified: Wed, 10 Nov 2021 19:47:19 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2048ab5bcdf748f8ad3fa69c37872412e50890aa8e11be31cba1d11d336df43d`  
		Last Modified: Wed, 10 Nov 2021 19:47:19 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe944376084c159a0107b88997b7c5ee8580fa57c0f9d700c3e6af759ac6143b`  
		Last Modified: Wed, 10 Nov 2021 19:47:17 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cdf339bd791d7a1fb8d99d3fd8c36b95248a8c43560050a07ae07e30b71601`  
		Last Modified: Wed, 10 Nov 2021 19:47:58 GMT  
		Size: 233.7 MB (233670831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe86018a2be9aacf394f6ffa369a25403d2a0bba327984d2c54b971812be182`  
		Last Modified: Wed, 10 Nov 2021 19:47:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63ce3bb0027cfc6013b99608e87689c84ea0c1d775cca64e32ed06b40b835a2`  
		Last Modified: Wed, 10 Nov 2021 19:47:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71896b3d7f2b4a8205fc17aeb251b55c0a46b1cc7b67898af8ba91f5eb932f4`  
		Last Modified: Wed, 10 Nov 2021 19:47:17 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
