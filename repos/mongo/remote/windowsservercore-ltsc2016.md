## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:9b10e750e189bcc91d4b8b437df5d0e1916a1bbd83da5804c77a6dc8f614f57c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull mongo@sha256:dc1e0e0a746355d51b918456ead65b0c79be3ff8079c5abe5557155df531807e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6574165890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fabaeef57593c53613c914f16da5a21ab483334c223dd0181771dd7922a947f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 01:55:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 08:12:35 GMT
ENV MONGO_VERSION=5.0.5
# Sat, 18 Dec 2021 08:12:36 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.5-signed.msi
# Sat, 18 Dec 2021 08:12:37 GMT
ENV MONGO_DOWNLOAD_SHA256=a791d7197849516381b3dc5b2ebb988432b95b52e347a3ce3d70d026d108886a
# Sat, 18 Dec 2021 08:15:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 08:15:09 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:15:10 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:15:11 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6bffd19db3f71ba2031bea25a529c67034869e7e1bbf9e2431d5ee747bd6d6d`  
		Last Modified: Sat, 18 Dec 2021 04:00:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b6a4e3511527ee432f9826d8c4c513d3609e9e431ebab5b3db3719b128a8`  
		Last Modified: Sat, 18 Dec 2021 09:09:14 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92c90c06db456b01aa86e6254292c16a7a7a4405c11c03270196b1b9454825c`  
		Last Modified: Sat, 18 Dec 2021 09:09:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3098383fc3df97f824b2af6a7e37c4b507f6ef5fbf0cc41c58aad7d2080d0`  
		Last Modified: Sat, 18 Dec 2021 09:09:12 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d339318b7144c3383db6dfcdf8c4be1c10fa1759f4045f7edf576875314bdf93`  
		Last Modified: Sat, 18 Dec 2021 09:14:27 GMT  
		Size: 299.4 MB (299441294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c550530f6a1130a48bff85c005030630f7d9fac99524481b9948c753a38eb15`  
		Last Modified: Sat, 18 Dec 2021 09:09:12 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0b2912a429910c0a9e5a57300ddd9c8388d64c6b056433c3cf906f1b1006fa`  
		Last Modified: Sat, 18 Dec 2021 09:09:12 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9273e0179936d4372d24a64f54fbda2084f6c348d685f86560b2957a2020202c`  
		Last Modified: Sat, 18 Dec 2021 09:09:12 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
