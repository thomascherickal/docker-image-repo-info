## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:13b11848469d499c0f47c7b7ba319025ecac7c638fc74193369fe6d35c7dae77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull mongo@sha256:f0534dfb20d90f152a7b4ae8812c61381cff7de983c2b17fc1fe3558a237fdac
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6023738394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df09b12dff596c207467d06492c25f69160b4857e5ed936f22e5b56e28f0d31`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 15:29:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 14 Jan 2021 00:26:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Thu, 14 Jan 2021 00:26:52 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Thu, 14 Jan 2021 00:30:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:30:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:30:54 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:30:54 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b5ee02f83739eef6745d432d63363ce5f490820d4b3e39ae83aa4e3771c4073`  
		Last Modified: Wed, 13 Jan 2021 18:32:39 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d389be6d2b8ed20cd152cea9411d21a4d5234844204ee0fd90f9479072198e`  
		Last Modified: Thu, 14 Jan 2021 00:58:39 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e36329a15f611a7f2bc62bb61ef59d2ca7682d5e0fd6e53afa9d410f578392`  
		Last Modified: Thu, 14 Jan 2021 00:58:37 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74af836ee8356e23ea2f57b2f34a678f2896d65398558032248d3bf4062ba94`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ea8f8ef27e8c66533eb49ba20bf1a04fd5dba5b9e7be779210d066c891c08c`  
		Last Modified: Thu, 14 Jan 2021 00:59:26 GMT  
		Size: 229.8 MB (229836266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67bc9d76410b618f3b32e1226468ad4a2411a7b855c2a4f1ad38f2fcc75b41`  
		Last Modified: Thu, 14 Jan 2021 00:58:35 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb38cc0511c79b847573aa38edf1e13c021a7befa0b7502681bed33d26b7912e`  
		Last Modified: Thu, 14 Jan 2021 00:58:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7b388ccf640debaf4477f3b825f6594e108d18d61068ea7264786b58a9297`  
		Last Modified: Thu, 14 Jan 2021 00:58:33 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
