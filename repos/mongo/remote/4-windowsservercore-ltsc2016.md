## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:bb52e87b2d69cb7674aba428e94e324094634beedb2748eb0e665a54cf90ef20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull mongo@sha256:44779078cdcab5eaa997e18b4ca88586d442ac26ee4663de3af1a4f891b954d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6503629014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3440e4e4fb49ba03f6c3e66461c79a7961deb6692d7da7ac04d984a5962c1d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 20 Sep 2021 22:22:01 GMT
ENV MONGO_VERSION=4.4.9
# Mon, 20 Sep 2021 22:22:02 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.9-signed.msi
# Mon, 20 Sep 2021 22:22:03 GMT
ENV MONGO_DOWNLOAD_SHA256=aa2eef8fbf94a91428da1ec9cd61acd7e44612e2ae35ae616aefe0a8f93cf282
# Mon, 20 Sep 2021 22:24:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 20 Sep 2021 22:24:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 20 Sep 2021 22:24:07 GMT
EXPOSE 27017
# Mon, 20 Sep 2021 22:24:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8a890dfb23ade347fae326bf6cadb29514ab1097d4433602c55995135becac`  
		Last Modified: Mon, 20 Sep 2021 22:45:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82d59e9be4e07d79899ac44c8fc2975d5ead38e16fe9e1c7ab02636e4645de7`  
		Last Modified: Mon, 20 Sep 2021 22:45:10 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e09c1ffea1e5c7bc006c0f26328ac86dbdfc2443173c079c468f9fcb0f5bfbb`  
		Last Modified: Mon, 20 Sep 2021 22:45:08 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116612afda4d630edb51683e0344ddd2d8963de874201a5690b76d3d0c0afd95`  
		Last Modified: Mon, 20 Sep 2021 22:45:48 GMT  
		Size: 232.3 MB (232290959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3723bdd66f5f624a77eeea6ca26573ffc7720da8d781640a726bb31fd7cddc47`  
		Last Modified: Mon, 20 Sep 2021 22:45:08 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723c000e87668586f2556e4f919b6e45c8080415f072bafb8c67ce48b4e444e`  
		Last Modified: Mon, 20 Sep 2021 22:45:09 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d828bade47fb0aadf008465a3a2ed44d16f2b67dc7cec8555feb7a6776cb4673`  
		Last Modified: Mon, 20 Sep 2021 22:45:08 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
