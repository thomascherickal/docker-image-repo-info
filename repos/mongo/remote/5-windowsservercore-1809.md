## `mongo:5-windowsservercore-1809`

```console
$ docker pull mongo@sha256:4e64b3de8d8c38500086b436e2ea803e159514e0a533474151bfbc192d7ca217
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `mongo:5-windowsservercore-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull mongo@sha256:ab03b66e493945ef56e8a58753a16c7165d1a3e0b049f3445669e3c52c2a6c56
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (3003640307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67beafcc8debb0bbb6a4edd3af66d7555fd4888f0ad9a0ed9dbf12908b55d293`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Sat, 18 Dec 2021 01:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 08:09:53 GMT
ENV MONGO_VERSION=5.0.5
# Sat, 18 Dec 2021 08:09:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.5-signed.msi
# Sat, 18 Dec 2021 08:09:55 GMT
ENV MONGO_DOWNLOAD_SHA256=a791d7197849516381b3dc5b2ebb988432b95b52e347a3ce3d70d026d108886a
# Sat, 18 Dec 2021 08:12:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 08:12:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:12:24 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:12:25 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d22d2238b031d3f13bcd6c144e80f8f8402332b8ee8e53cc54b7912c3ac808cb`  
		Last Modified: Sat, 18 Dec 2021 03:59:34 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e86d8cc5d7d638007d4f46887284c38c260aa8f7f897c9e33be0ebf643fc3d`  
		Last Modified: Sat, 18 Dec 2021 09:08:04 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a41ae0d046213a6456bddaef63c04cde17e326404faf2583ee4aedb0e8be4fc`  
		Last Modified: Sat, 18 Dec 2021 09:08:04 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890eb1acbec3565f478a644c9504860dd1576558ac6b1a8c8e2015317ba72416`  
		Last Modified: Sat, 18 Dec 2021 09:08:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2570c731cc6a4b6640fa9e3926b0dc2a3f223d70b679c0e334cd78ace09350`  
		Last Modified: Sat, 18 Dec 2021 09:08:57 GMT  
		Size: 295.0 MB (295025913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585d9711a8402e4ae77e4fec4694213e8e00c24f61a58b522c47041357112013`  
		Last Modified: Sat, 18 Dec 2021 09:08:02 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d9af230e33712a77bcffa99e1f63ce62decea4885299bb26540661e5929b2f`  
		Last Modified: Sat, 18 Dec 2021 09:08:02 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e45273e91eff42422f7946f4ef1c2fb913f2f8359515365a42121a8464cf72`  
		Last Modified: Sat, 18 Dec 2021 09:08:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
