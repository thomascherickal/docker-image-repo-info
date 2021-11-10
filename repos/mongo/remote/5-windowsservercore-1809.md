## `mongo:5-windowsservercore-1809`

```console
$ docker pull mongo@sha256:4e553e6403311dc73b448e357537bcd9235d6beb0126f8e7e6eed1d155f42cfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `mongo:5-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull mongo@sha256:81925d1694621985a0da6dfc3d6ba8754bdb7cca0aa95c11e295135fea9ea8cb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2999326674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04977edae162f4f32904979581c7b7b2cdeaf8d513d6e113548454a34f4ef7a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 14:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 19:09:15 GMT
ENV MONGO_VERSION=5.0.3
# Wed, 10 Nov 2021 19:09:16 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.3-signed.msi
# Wed, 10 Nov 2021 19:09:17 GMT
ENV MONGO_DOWNLOAD_SHA256=ed1cc2eee23f4fb9cc7f70867e29d7c9a1e1af1d9b4aa917d247a4921c4ffd7e
# Wed, 10 Nov 2021 19:11:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 19:11:17 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Nov 2021 19:11:18 GMT
EXPOSE 27017
# Wed, 10 Nov 2021 19:11:19 GMT
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
	-	`sha256:73352456d792898cf9b7bd0e190b4bc8aa72dd6840f210fa6f76bdb0b354afc7`  
		Last Modified: Wed, 10 Nov 2021 19:34:14 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d4ce8e69782f42c9e5dcab71eef5f25aff7d411e1fedfe2a7f31bd910dd72e`  
		Last Modified: Wed, 10 Nov 2021 19:34:13 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c216118dfb955e9ffe5cb0a0b988836f50af00f8189e641886b7140c7f725585`  
		Last Modified: Wed, 10 Nov 2021 19:34:11 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e20eac49644f1e2f06b23faa271f9f79ece770f97c554902351402e77a56c51`  
		Last Modified: Wed, 10 Nov 2021 19:39:34 GMT  
		Size: 293.2 MB (293195920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cbf1ae731655ab222703a5c735751c041291bffcd76ede9da1ddd8152396c2d`  
		Last Modified: Wed, 10 Nov 2021 19:34:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d8a7c5c1948759c44add877514317c2c9937ef4c21752e5e0c374b14803421`  
		Last Modified: Wed, 10 Nov 2021 19:34:11 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14264e01ffeaab1d5d4d9f8baf90b5361057c5a357dee2ee73e5604d0504fc79`  
		Last Modified: Wed, 10 Nov 2021 19:34:11 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
