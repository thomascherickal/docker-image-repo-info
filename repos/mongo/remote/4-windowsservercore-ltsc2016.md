## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:0522ce9995282b1ebcdd1ec126a2bf0270c311707dd7bbfd18682c2f2d02ae73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull mongo@sha256:b73b2ba81f9b1ff35543cb16245b4a4c975d6bc667b6e4a6e82a595e4117d5cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6507509954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0143be1883bc53aca702dc26310eb32d384c264fe7ca08f6e725510e115e8bc7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 13:57:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 21:36:40 GMT
ENV MONGO_VERSION=4.4.8
# Wed, 11 Aug 2021 21:36:43 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.8-signed.msi
# Wed, 11 Aug 2021 21:36:45 GMT
ENV MONGO_DOWNLOAD_SHA256=b66e3beafa5623eced86f0a7298932918ccd27199e572021f7e8ea074cc51f23
# Wed, 11 Aug 2021 21:39:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Aug 2021 21:39:44 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Aug 2021 21:39:47 GMT
EXPOSE 27017
# Wed, 11 Aug 2021 21:39:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d6d4b60a6f3b0544427c2eb9a5e27e5f6ddca0fd7632003e11331f01c4e9c6fc`  
		Last Modified: Wed, 11 Aug 2021 16:25:34 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f782df426f6538663d9aa787495813d0e0ca4a532d1e73824a7c94c485dff59`  
		Last Modified: Wed, 11 Aug 2021 22:02:34 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fbd43828507b1e3d74a006591a58e411336660f6465e01fba849727b51503d`  
		Last Modified: Wed, 11 Aug 2021 22:02:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588527b09a6cb018e8d65c8836e625e2bc70ae32d19839e36aa428474092d104`  
		Last Modified: Wed, 11 Aug 2021 22:02:32 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5033ca6ec7874a4bb83d51ca1209dc9f9c71a90b533da013772778a1ec5dfa96`  
		Last Modified: Wed, 11 Aug 2021 22:03:13 GMT  
		Size: 236.5 MB (236533899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9861995f33bd288e6fef80fc7fc466819c1475a0700a6b89e0bd6bf18a155304`  
		Last Modified: Wed, 11 Aug 2021 22:02:31 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3bb6e99b70f978d557ffb4ec65f0f979a37e8873e6f33145ff5d8c5a62c777`  
		Last Modified: Wed, 11 Aug 2021 22:02:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5a39faed2ccb022dd811b3b01bc6cfe4756f7191476926da18eb70397105fb`  
		Last Modified: Wed, 11 Aug 2021 22:02:31 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
