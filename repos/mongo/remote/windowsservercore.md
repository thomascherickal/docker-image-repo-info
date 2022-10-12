## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:e0e4036ca1cea9feb7ccb957ec233f8ec5e1b8234085d1e6dec1e7fecb70b31e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1129; amd64
	-	windows version 10.0.17763.3532; amd64

### `mongo:windowsservercore` - windows version 10.0.20348.1129; amd64

```console
$ docker pull mongo@sha256:9f0124900745a02043158bec64db08934598aed691eff9b313a975930a1ab9cc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2928919101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f75bf702de10b4f40ad8964f5bdaa684e62d98feed607baf785fbcb255b7007f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Wed, 12 Oct 2022 13:23:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Oct 2022 17:07:21 GMT
ENV MONGO_VERSION=6.0.2
# Wed, 12 Oct 2022 17:07:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-6.0.2-signed.msi
# Wed, 12 Oct 2022 17:07:23 GMT
ENV MONGO_DOWNLOAD_SHA256=964a7e33927a8c01a6177daf0bf49f3ec17560b1b78f8be60ec641a03c55cb18
# Wed, 12 Oct 2022 17:09:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 17:09:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Oct 2022 17:09:20 GMT
EXPOSE 27017
# Wed, 12 Oct 2022 17:09:21 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:81f8c9039f908cbcc912779f9e4c8c5ef145be551538af133f6a9e98c284e2c2`  
		Last Modified: Wed, 12 Oct 2022 14:57:06 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e33316874e96cca28048b1ef4278c583b132be32d3249f6ea78c78385dc1b3`  
		Last Modified: Wed, 12 Oct 2022 17:41:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269dfbb34bb45e2c569b49f31b03cbf5fcd75d896233851d92b8a05337d93b72`  
		Last Modified: Wed, 12 Oct 2022 17:41:56 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61182a2e145436d402b4cda85b23d80acd1b81bc58329c517fb125e2c735c11`  
		Last Modified: Wed, 12 Oct 2022 17:41:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cd2e92dc993212dbc329b6f7e1bb7c60b7539fd9361ac039ff2a89494d56ef`  
		Last Modified: Wed, 12 Oct 2022 17:43:18 GMT  
		Size: 512.7 MB (512685908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27787617cbd4b0dc9c87d024c1fb08896b5cdaa18007b07d3f83e29929819e35`  
		Last Modified: Wed, 12 Oct 2022 17:41:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b239164ce10fd9be5b8f93faf270cf0abe79a73f11368fbd3404bbb980f59b3`  
		Last Modified: Wed, 12 Oct 2022 17:41:54 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca04e10644a32bd270c53ee57e9044f61bea611e31447e9b4aca0fa74d9f563`  
		Last Modified: Wed, 12 Oct 2022 17:41:54 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull mongo@sha256:e9cc836d8b27bda179ccb5f98c53c51b94d35cf1c5f3c71e10a761480181e3e4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 GB (3223653636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d66de17796d800a70082f5398c0fc69393e464229b8fd8e7a99e375ae93a1a81`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Oct 2022 17:09:38 GMT
ENV MONGO_VERSION=6.0.2
# Wed, 12 Oct 2022 17:09:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-6.0.2-signed.msi
# Wed, 12 Oct 2022 17:09:40 GMT
ENV MONGO_DOWNLOAD_SHA256=964a7e33927a8c01a6177daf0bf49f3ec17560b1b78f8be60ec641a03c55cb18
# Wed, 12 Oct 2022 17:12:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Oct 2022 17:12:32 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Oct 2022 17:12:33 GMT
EXPOSE 27017
# Wed, 12 Oct 2022 17:12:34 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1078c1a99ba07ad73a4e126d6581d11638f76c357e28c3eb681efd9cfee011`  
		Last Modified: Wed, 12 Oct 2022 17:43:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7ae69d61efab1b59e67a4700c9e9b0c0b0eafe8a8cd4716232bb2026029705`  
		Last Modified: Wed, 12 Oct 2022 17:43:36 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8870889cb57eba8c443d18b1b134d50416c81dba93e7f9e4247349e9ff47e41`  
		Last Modified: Wed, 12 Oct 2022 17:43:34 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9895666b3b625ce83fa3d38516b691a9b63c5a09981c1d3578b2c0938f921f`  
		Last Modified: Wed, 12 Oct 2022 17:44:49 GMT  
		Size: 512.5 MB (512480197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4133c0cf3dbc96c0edbb9dd37b38e240a5e75b250b0d39262da8fef8a029f1c`  
		Last Modified: Wed, 12 Oct 2022 17:43:33 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0eded977a45e28cb7062c482f62ff5e94eb85cb410b44c67d9f334e4ff91ad`  
		Last Modified: Wed, 12 Oct 2022 17:43:33 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbeed7a7903a3a89688e0a6507ee56f687fd147d5010c782f9f380bb6e6e9460`  
		Last Modified: Wed, 12 Oct 2022 17:43:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
