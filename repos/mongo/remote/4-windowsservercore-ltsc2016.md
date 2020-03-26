## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:4b0434a00c72fc81e0fbf7fc85648f3c003b2fe5512f04865efbc80fe7dfca29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull mongo@sha256:cc9001a843603f7cf6e32e975d86f0cc6464bb6f17d3a5dc90749cb3c6512790
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5825372001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8f44b45694426f4ed3ecdd6ece4bbb4a0f02a94f402849c65fdf20e05ba9f32`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 26 Mar 2020 19:15:50 GMT
ENV MONGO_VERSION=4.2.5
# Thu, 26 Mar 2020 19:15:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Thu, 26 Mar 2020 19:15:52 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Thu, 26 Mar 2020 19:29:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 26 Mar 2020 19:29:44 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 26 Mar 2020 19:29:45 GMT
EXPOSE 27017
# Thu, 26 Mar 2020 19:29:47 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10f5bdc11bba6335ddf686dc4b683b602ffdcc9d7be0a07602aed3897c95c8d`  
		Last Modified: Thu, 26 Mar 2020 19:49:41 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464ddc4d13a7a3db9e69062ad56eb9a0e5d5d020a0bf1e852ebf21a675420891`  
		Last Modified: Thu, 26 Mar 2020 19:49:42 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1316fb62770395a7b841083b9e28a65f743f0318f8060a2ff312e0e62dc1bb94`  
		Last Modified: Thu, 26 Mar 2020 19:49:38 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ab0831770bcdf202c89efd9cc1e09a57ae7defad2134eb96a1663fa014c61c`  
		Last Modified: Thu, 26 Mar 2020 19:50:01 GMT  
		Size: 96.6 MB (96602951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f2e63ca5b93cecb8429488d5d13beb3acf51b941c747dd586c0e6b4f2fb21b`  
		Last Modified: Thu, 26 Mar 2020 19:49:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e035d36f8280b5d5a5dd1a3da0bde53aa807133388a34cae298c58b1fd5bbe14`  
		Last Modified: Thu, 26 Mar 2020 19:49:39 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480372cecef792ea73320c6616c008444718def7efaa1e41fc4385cea1d3ed88`  
		Last Modified: Thu, 26 Mar 2020 19:49:39 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
