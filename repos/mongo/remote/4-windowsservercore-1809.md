## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:2e06fba0b40fd8ba31c9f9aba87e63169fa4c566760c6ac1ff62e70bcf29c0ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull mongo@sha256:b0e302895ad27d4370da368631ad28dc59ed5decec75e6abdc51c8705d8412e8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2955903819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53715fe136c6528382aecebb86ae88f1acd507a1de8e2085838a22d8050fb329`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 17:05:23 GMT
ENV MONGO_VERSION=4.4.12
# Wed, 09 Feb 2022 17:05:24 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.12-signed.msi
# Wed, 09 Feb 2022 17:05:25 GMT
ENV MONGO_DOWNLOAD_SHA256=a46ddabb46813c509555bdb012e34f0aadd12b5348a23ad7206fc18ac5a2fcd0
# Wed, 09 Feb 2022 17:08:19 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Feb 2022 17:08:20 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Feb 2022 17:08:21 GMT
EXPOSE 27017
# Wed, 09 Feb 2022 17:08:23 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76c4b6870ab21985e40c2b40d58fbcb5ddf96549ce78fa2e3eb82a24aa55f8f`  
		Last Modified: Wed, 09 Feb 2022 17:51:00 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa298f42af79a8ce9070e6973f3b7221d5a80def3d1d958e687b12f4e7af4b6`  
		Last Modified: Wed, 09 Feb 2022 17:51:00 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a0006499f6d3247779d14683ca3bfa462484742ec68df7e0bb91a9493b87a3`  
		Last Modified: Wed, 09 Feb 2022 17:50:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c1c8c170184b71ca298f7895aa3ccc2a6b2241a4a6b73c96c91a1af2cfdee2`  
		Last Modified: Wed, 09 Feb 2022 17:55:20 GMT  
		Size: 242.2 MB (242179224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55223b62440eff09c1ccdd779dd4a7309158d5f4fd1d88aa6cc0109025608cb6`  
		Last Modified: Wed, 09 Feb 2022 17:50:58 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a8b4a4824cd0b3b3b45eaf6d74348be472453b7183cef9d4c14190977ab976`  
		Last Modified: Wed, 09 Feb 2022 17:50:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495b9f7341fa15c984a7e91dcf4e45e9803d78a8374c384c47b47c891f9850d8`  
		Last Modified: Wed, 09 Feb 2022 17:50:58 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
