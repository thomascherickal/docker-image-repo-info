## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:e529ecac82777d5fe4fa4a04d910ae0e5e504e7e63ae56e23a5b14a578d11d41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `mongo:4-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull mongo@sha256:8ca59fa742b80ad8bc7d6c25268732cf1587baa8dd42761223242a1f5630e40b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2918142511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:437137b89d1d4416dd0eea459db524710a1bb78c8e89bf7a5e5b47dfa1dd79b1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 13:42:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Aug 2021 21:33:57 GMT
ENV MONGO_VERSION=4.4.8
# Wed, 11 Aug 2021 21:34:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.8-signed.msi
# Wed, 11 Aug 2021 21:34:03 GMT
ENV MONGO_DOWNLOAD_SHA256=b66e3beafa5623eced86f0a7298932918ccd27199e572021f7e8ea074cc51f23
# Wed, 11 Aug 2021 21:36:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Aug 2021 21:36:27 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Aug 2021 21:36:29 GMT
EXPOSE 27017
# Wed, 11 Aug 2021 21:36:32 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c613f4c34660a122de754415a884afe6b12172ac3ce792a2e4aae831cc8b2e27`  
		Last Modified: Wed, 11 Aug 2021 16:25:11 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2938e4ca122e713d2ebf1520f83df4446904be2ba58dd81439acd8999b9d26f`  
		Last Modified: Wed, 11 Aug 2021 22:01:39 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6890c321dd9621ef8cf53d4181c7295cb43281e4585407da01c3c35abc346dd`  
		Last Modified: Wed, 11 Aug 2021 22:01:39 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf5bd432ed25d4222c9be5693adc3a1a76cdf0f171005c8bdb920a0a13aa93e`  
		Last Modified: Wed, 11 Aug 2021 22:01:37 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7514eca55883eb734a5924008e0f295d2a4ceeb20151e3f4b65f775d68a0205`  
		Last Modified: Wed, 11 Aug 2021 22:02:17 GMT  
		Size: 232.1 MB (232134663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92840a2cc56aa1a462cd78de94c5c26f071f3fd03bbb762f0b68ff48702ebb2f`  
		Last Modified: Wed, 11 Aug 2021 22:01:36 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b48167a465a11b7a8f6616793e297214ea0f1b1e73a18dd90053e3b730f1f80`  
		Last Modified: Wed, 11 Aug 2021 22:01:37 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f81622bf6f94395cf139db58d56edfa5f89ab6a26f4e1ee14fadc72ec7981c5`  
		Last Modified: Wed, 11 Aug 2021 22:01:36 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.14393.4583; amd64

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
