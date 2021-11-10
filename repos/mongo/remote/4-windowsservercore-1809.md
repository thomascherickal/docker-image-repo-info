## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:3f8aa9fccfa2c9ccdd7b4b4598ba238e7bd06552d4826bccaa70ae2286b6abd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull mongo@sha256:0aefb5538a0f0211472bceb5871aa90745248db389595a17b09acf2ee02d7245
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2939871053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a72204f30fc86d6f5afef2fb3b7a5c2979b0a29d30c8738e6d4c9429cbbbc9c4`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 14:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 19:15:26 GMT
ENV MONGO_VERSION=4.4.10
# Wed, 10 Nov 2021 19:15:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.10-signed.msi
# Wed, 10 Nov 2021 19:15:27 GMT
ENV MONGO_DOWNLOAD_SHA256=b48fbc7ba392f505a89af03301ed8f3f99b35c6ee8f3c9595cfebacf26ba68ee
# Wed, 10 Nov 2021 19:17:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 19:17:27 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Nov 2021 19:17:28 GMT
EXPOSE 27017
# Wed, 10 Nov 2021 19:17:29 GMT
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
	-	`sha256:62a0e4a52702a01f3004172de1c1dceaf4a842245160ac1bf9ab8f9d871c856f`  
		Last Modified: Wed, 10 Nov 2021 19:46:26 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7b47224aead9da1eb02fcf69a0febbbf11258f46f9c3eda61c2778829f83bc`  
		Last Modified: Wed, 10 Nov 2021 19:46:26 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108366249dc40ab345d0015da1c589bf5ce54d99d29ff4a0a3b1574caa9ed0dc`  
		Last Modified: Wed, 10 Nov 2021 19:46:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc2bc6044e512ce525ab810484d40d6312f1c4d0d2658a3d5ae9b646dc197f8`  
		Last Modified: Wed, 10 Nov 2021 19:47:04 GMT  
		Size: 233.7 MB (233740019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3740e4fc22ec6b07e888570ca595b6a42d5d6502d83e97424f794e4374349f`  
		Last Modified: Wed, 10 Nov 2021 19:46:24 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb76928049f8f39e96a7d9aac8644077aebdb6b19c2b18c3b14834a55081359`  
		Last Modified: Wed, 10 Nov 2021 19:46:24 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652dc1bc0b33ba198fb7fc673711f19b4feeb2bfba82731f48aaec7fd885d748`  
		Last Modified: Wed, 10 Nov 2021 19:46:24 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
