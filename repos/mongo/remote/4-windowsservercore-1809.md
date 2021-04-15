## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:2ef46fae28c381cf90b781605694e691bfb581bc4915bbaf95bb42a748029d49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull mongo@sha256:d0bfb8f110aaf97fdd185e13ecce83d51bf126af99a0da2c796fff4e9c140f83
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2706114849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6113a5a3a3992a2388a6006d91cc2a61393d1f0cfc737a7930d22c5b1f13aef7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 20:57:50 GMT
ENV MONGO_VERSION=4.4.5
# Wed, 14 Apr 2021 20:57:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.5-signed.msi
# Wed, 14 Apr 2021 20:57:53 GMT
ENV MONGO_DOWNLOAD_SHA256=1ef4f41cfaf3b91dc34543186b0b02ea2756075f4df822180b1fb46602604fd6
# Wed, 14 Apr 2021 21:00:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 14 Apr 2021 21:00:24 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Apr 2021 21:00:25 GMT
EXPOSE 27017
# Wed, 14 Apr 2021 21:00:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d85a16caeb092c2cd5c60f5eb2d6f1af7bee7e2f5d64b3e4ddafe8baf38e09`  
		Last Modified: Wed, 14 Apr 2021 21:23:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dfb153e69f5bea3c73510190f85bdbf719d37edb569710d2c98461dfb2c012`  
		Last Modified: Wed, 14 Apr 2021 21:23:58 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c54b9304ed5eee39543b56757f815059b23cdad4e2d05b5431c367778d670a`  
		Last Modified: Wed, 14 Apr 2021 21:23:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a08ba76942b7da68614b5549fea9b1ec7fde0d9ba10d49d3ffa971da0d28b6e`  
		Last Modified: Wed, 14 Apr 2021 21:24:44 GMT  
		Size: 236.4 MB (236350951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879cfbb57bca81670f888981ccdc26e234186a16c780893c33b2c7c314051eb8`  
		Last Modified: Wed, 14 Apr 2021 21:23:56 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ce3ba54554036747a56ad94b2b2b907fb5e646454a8996bfd366290e497bed`  
		Last Modified: Wed, 14 Apr 2021 21:23:56 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d63b5df074602137980550b3b2ac89e3f3fce4af02085b14fb2f5abe70f928`  
		Last Modified: Wed, 14 Apr 2021 21:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
