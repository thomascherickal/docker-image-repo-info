## `mongo:windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:8cc03f530dfb4648b7c4c47da54cf093e20c7f0e3ef8853c21e1cddd8d1dc46b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1850; amd64

### `mongo:windowsservercore-ltsc2022` - windows version 10.0.20348.1850; amd64

```console
$ docker pull mongo@sha256:0ff9a8cd70614e143b048d42edc771d9e8195768a963732974daf5b11e811737
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2255119873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deb5a6b9ac471917d203c486d53eff390eca4e62d29d3b0112baa33a33db3839`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 07 Jul 2023 21:29:32 GMT
RUN Install update 10.0.20348.1850
# Thu, 13 Jul 2023 22:35:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 13 Jul 2023 22:51:52 GMT
ENV MONGO_VERSION=6.0.7
# Thu, 13 Jul 2023 22:51:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-6.0.7-signed.msi
# Thu, 13 Jul 2023 22:51:53 GMT
ENV MONGO_DOWNLOAD_SHA256=41dabd0f59813c675f6973201374800b300800060839968b9fda7371423061b1
# Thu, 13 Jul 2023 22:53:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 13 Jul 2023 22:53:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 13 Jul 2023 22:53:49 GMT
EXPOSE 27017
# Thu, 13 Jul 2023 22:53:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a7416e1317a892f4786a89c62493b21df55e0e06b82a4bb007cc79df0f949`  
		Last Modified: Tue, 11 Jul 2023 18:03:32 GMT  
		Size: 348.8 MB (348766456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2bae42a1ce047820c1f128e4587a430377ba56a110db0d98ec3ccfbd3de58a`  
		Last Modified: Thu, 13 Jul 2023 23:23:36 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed35bb27c3558d6110bcd48c86daea76058dd886732871d20981324b009bc99`  
		Last Modified: Thu, 13 Jul 2023 23:36:13 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2fb9d3eae62d5831e14ad1e2e3931b04f4bfceb01adf953dd347bc5c4a0525`  
		Last Modified: Thu, 13 Jul 2023 23:36:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569719a1dc7eef279ed34c32b784f8a4dada4dc89e3f3895cc146176d3b5b0b2`  
		Last Modified: Thu, 13 Jul 2023 23:36:11 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e52264f4872a71b0dd4eaeabb0d9e6c24bfa426c1428c0909c22b1f498e554e`  
		Last Modified: Thu, 13 Jul 2023 23:37:29 GMT  
		Size: 517.7 MB (517744688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3768693df91813631fc4f6d4fe0f3b1e0c8d14ef2cf1d035745bebe888b49558`  
		Last Modified: Thu, 13 Jul 2023 23:36:11 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce1c9b448183354ed9d5ae50932e6bde28bf51ca035fefdbcd2a445f5ba6bdc`  
		Last Modified: Thu, 13 Jul 2023 23:36:11 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d64206ad5d9a890d6fcf65a07d87d15b296ef02fdc289e5677afa12ff42baf`  
		Last Modified: Thu, 13 Jul 2023 23:36:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
