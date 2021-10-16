## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a988dc641420fadaad06f6f0f5599107215fd526cdd0b0b0434cf3f35ac6655b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull mongo@sha256:4a33726f34141d123572c890074482392342d82ece6655368143a6608c96fd73
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2920073189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28831036cb72777754e1e872f1741e5b46a1d53ed4d6766bf06d7f793b144157`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 00:34:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 16 Oct 2021 00:15:53 GMT
ENV MONGO_VERSION=4.4.10
# Sat, 16 Oct 2021 00:15:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.10-signed.msi
# Sat, 16 Oct 2021 00:15:55 GMT
ENV MONGO_DOWNLOAD_SHA256=b48fbc7ba392f505a89af03301ed8f3f99b35c6ee8f3c9595cfebacf26ba68ee
# Sat, 16 Oct 2021 00:17:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 16 Oct 2021 00:17:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 16 Oct 2021 00:17:52 GMT
EXPOSE 27017
# Sat, 16 Oct 2021 00:17:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55c74bf8af074a49872e1e0411ac5572625083d17cb1100c5cade611deeb92ff`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee99c653d65c7568e026483203994e9f9e6492798ed148e334b741606db826`  
		Last Modified: Sat, 16 Oct 2021 00:22:54 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3176f62e247c35fc76e7b94d40da421730f444d49eaa16fa7c154b7385b3be55`  
		Last Modified: Sat, 16 Oct 2021 00:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2819da8555d0b775de0bea47164dd3ac302d51144c3a1879b521df4ef5238fd`  
		Last Modified: Sat, 16 Oct 2021 00:22:52 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e6cffc05ccd817d45f87e0fbe317257bfe723d377a5b2cd4e451dd6d4b0e11`  
		Last Modified: Sat, 16 Oct 2021 00:23:33 GMT  
		Size: 233.7 MB (233744607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303379468feba0d71bda89f23854db0aed47b305a56f4823b96bd30bcfef29e6`  
		Last Modified: Sat, 16 Oct 2021 00:22:52 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e1f6683fe2d5b98d768c36a89bfcdff581d0e8f6bb2ad44a705f8d72ba71bf`  
		Last Modified: Sat, 16 Oct 2021 00:22:52 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81fc3729badb4b8372df5d044f439729447a3419f1281e333aea48263dcd2cb`  
		Last Modified: Sat, 16 Oct 2021 00:22:52 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
