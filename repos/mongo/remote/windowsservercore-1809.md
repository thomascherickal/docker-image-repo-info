## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:ad53239422ffa32c13fa26e69de972bf42066eaf685af5bed21512ca58d90d9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull mongo@sha256:5a2f10ff220ec8f3786d2a074a0684e4d6107be5c7b612441cab9c7429a9a8bd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (3001038601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e1c31364e7ad42a3bc06369d7ec436baccd1fcd720a0b87e3d40de0dc6738a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 14:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Nov 2021 02:15:26 GMT
ENV MONGO_VERSION=5.0.4
# Tue, 16 Nov 2021 02:15:27 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.4-signed.msi
# Tue, 16 Nov 2021 02:15:28 GMT
ENV MONGO_DOWNLOAD_SHA256=f44191d6e1f187ee6ff5404f6095f8c8f621bdaca56e54099fd4d2266f4cb60f
# Tue, 16 Nov 2021 02:17:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Nov 2021 02:17:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Nov 2021 02:17:47 GMT
EXPOSE 27017
# Tue, 16 Nov 2021 02:17:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db1ba835bccbdc73ef254c175ca6ae0dc3f0bd759c1910c3b123cfb9613223be`  
		Last Modified: Wed, 10 Nov 2021 16:21:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c108852a4208e178f48e763e0b661a2d1ef8c785b95564747e42574d212e89db`  
		Last Modified: Tue, 16 Nov 2021 02:23:50 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ebab2821274a5746503dced26929e509a2a64135782dd17bdbdfe2aeefee6e`  
		Last Modified: Tue, 16 Nov 2021 02:23:50 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db26354b44ed31392a1c1660b5a8fd2508d9a1c131af31703414165a542d7ca`  
		Last Modified: Tue, 16 Nov 2021 02:23:48 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356893e64aa17aabb5c74c1b9f84065cc13adb29915d4a318dfc12722b15accc`  
		Last Modified: Tue, 16 Nov 2021 02:24:41 GMT  
		Size: 294.9 MB (294907527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd77ea004492d76397bd51d2d153e6fffeedf18faacd16722590ba3e5635095`  
		Last Modified: Tue, 16 Nov 2021 02:23:48 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7019136d393e3ef719f87f544d191cf18e770df615dda3a79ab461fae93098c`  
		Last Modified: Tue, 16 Nov 2021 02:23:48 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbe252158c193ff148432fc8ca800e2e1e14df0a2271a4436a1d4ea1c2879e2`  
		Last Modified: Tue, 16 Nov 2021 02:23:48 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
