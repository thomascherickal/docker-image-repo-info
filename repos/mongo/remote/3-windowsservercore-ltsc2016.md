## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:52630676efc96befa6e39413412ef130f145cdf478f6e886a6e8cc088ef1deb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull mongo@sha256:36a967b2327cfa45e973b881bd4a7934f06ebdd8363c6cf0b69ce7a45a321237
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5827645797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5257e6147460e9d6d88072bf34645b0726d3a4ac5ec84fad7b78b32ba0cd4d4e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 18:12:21 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 10 Jun 2020 18:12:22 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 10 Jun 2020 18:12:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 10 Jun 2020 18:25:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Jun 2020 18:25:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Jun 2020 18:25:56 GMT
EXPOSE 27017
# Wed, 10 Jun 2020 18:25:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fc06f25a20433529cc677026660803d286db9e3f8a055137e0fb4adf012f30`  
		Last Modified: Wed, 10 Jun 2020 20:26:03 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba0430b99800ae303becc127d856e491cee47840694a93137ff4b541ec3dd20`  
		Last Modified: Wed, 10 Jun 2020 20:26:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df886cb63add8ca65718c352acc3fb8eb0fe36b91664cf0656c582179826898`  
		Last Modified: Wed, 10 Jun 2020 20:26:01 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a205b8dfbf1b2ef64f36fecadd0bdd0a24da03ec7dd0d5c067973d40ea3c899`  
		Last Modified: Wed, 10 Jun 2020 20:26:21 GMT  
		Size: 93.6 MB (93640049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb4100f96204b1734a5f4ddffe022067cb3e48d70ed5079fc4a2e012da1185`  
		Last Modified: Wed, 10 Jun 2020 20:25:59 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecb46291fd9c779f2b145d5c49b5b9e9ff15565e32d19a059a4662e24db90ae`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc42606f221bf05aec5c472b015b8eb5e07704d8c498dbca5058adbd2eef885`  
		Last Modified: Wed, 10 Jun 2020 20:26:00 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
