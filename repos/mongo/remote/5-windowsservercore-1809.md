## `mongo:5-windowsservercore-1809`

```console
$ docker pull mongo@sha256:2b5fc3e5ba1981117b716ac9f4d7fdec1637fca852bd09f835f49a38f2767b91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `mongo:5-windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull mongo@sha256:1d01e4976e1145a44582f2119e724610e233416ba3f2e6df2c26061e3064f1d0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2275331280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:459b81cf7a6153e97db745bece27e80efdfaaa0e6c3b27a206bc88f6d2cd1946`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Thu, 16 Feb 2023 00:42:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 25 Feb 2023 00:18:08 GMT
ENV MONGO_VERSION=5.0.15
# Sat, 25 Feb 2023 00:18:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.15-signed.msi
# Sat, 25 Feb 2023 00:18:11 GMT
ENV MONGO_DOWNLOAD_SHA256=882dce3858f3580011cd295f5c6502a4effd19178968abd7c20f8aabb50a7c15
# Sat, 25 Feb 2023 00:20:51 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 25 Feb 2023 00:20:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 25 Feb 2023 00:20:54 GMT
EXPOSE 27017
# Sat, 25 Feb 2023 00:20:55 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531f6c3ad9784fc2870ea5ca08c4adccd9318602ed534d822e12b8b658a7b0b6`  
		Last Modified: Thu, 16 Feb 2023 01:37:30 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad280ba3cdba63405d80a68fbbc28665fc0b673fce991f09769433cc9a273400`  
		Last Modified: Sat, 25 Feb 2023 02:19:56 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:586997162aa31a6f4b54d59a678a32a561ff687e2b056e364e85b0937b8eeffc`  
		Last Modified: Sat, 25 Feb 2023 02:19:55 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2f2d613dbb207a5661691932472d166ba98e660085b233391073ac60b05bab`  
		Last Modified: Sat, 25 Feb 2023 02:19:53 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51df2cf5437761b25145acf66a7e110b7fac8d6277959c2f29029454577b77c`  
		Last Modified: Sat, 25 Feb 2023 02:20:50 GMT  
		Size: 312.4 MB (312363497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64cf84e6afecb5cbf3004f213427ffcd38bdcdec69390df0a80df87e9f6b2ceb`  
		Last Modified: Sat, 25 Feb 2023 02:19:54 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2893629d85dd9edb6752089f6b9adb48f127ba7c86f3b55e8066dba9974c1b5`  
		Last Modified: Sat, 25 Feb 2023 02:19:53 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3be78ea423c638a436cbf2ec18cf4cf96eef56255b336b76f2fd2ef189e081e`  
		Last Modified: Sat, 25 Feb 2023 02:19:53 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
