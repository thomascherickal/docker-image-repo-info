## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:6b30ee76be513f99e97774b0ba47b0130bc655f5ff933d5b6c05286cc0884fa4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull mongo@sha256:3ccc06161d7c01a15a5a41a2bcd7d2f01468e51d2b028198a1a0d48fe762f2bd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (3026048608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54b771614c2c58bb1c1a9aa382dc63df3cc2523bc108bdf31d893722c6a4fd45`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 01:53:43 GMT
ENV MONGO_VERSION=4.4.18
# Wed, 14 Dec 2022 01:53:44 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.18-signed.msi
# Wed, 14 Dec 2022 01:53:45 GMT
ENV MONGO_DOWNLOAD_SHA256=e647d6432ceaf4949bd989e10bad5cd10788f87c41ac2fc054a6e6122503fc64
# Wed, 14 Dec 2022 01:57:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 14 Dec 2022 01:57:31 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Dec 2022 01:57:32 GMT
EXPOSE 27017
# Wed, 14 Dec 2022 01:57:33 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580241097bd56ef79e0f9aab62b80cddc0b3d5b8c70dd16710b15f1dbcd18e50`  
		Last Modified: Wed, 14 Dec 2022 02:27:19 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d8887837425b21347f7536ef82cf6e1554f625470b8289dd6d1f899fdf02e4`  
		Last Modified: Wed, 14 Dec 2022 02:27:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036d0427c34e490a0ed7b79b1f5323002a2bce287540554b6cc566890de9e2cd`  
		Last Modified: Wed, 14 Dec 2022 02:27:17 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd5698fa1c75282fdcb25c6b33863d60680a55292114543979ffd1b1a635215`  
		Last Modified: Wed, 14 Dec 2022 02:28:05 GMT  
		Size: 245.3 MB (245341430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63ebb88793da573d5879356c230cfc511d472b8788f7f0a9f6c0a20b30132dc`  
		Last Modified: Wed, 14 Dec 2022 02:27:17 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86c4944b63f5b4320d830e028b863e26c3fdb04e2b33e8620d51d2350937461`  
		Last Modified: Wed, 14 Dec 2022 02:27:17 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f0972a0b0b5fe6a72f7323ebbf1eb071d75186a7198993152fe769693f53b1`  
		Last Modified: Wed, 14 Dec 2022 02:27:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
