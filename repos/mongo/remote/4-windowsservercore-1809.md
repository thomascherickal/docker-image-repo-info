## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a218b70c050ffcd70e88e2969459b0b990e9e0f4e32973a5e090ab7785ab7bcd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull mongo@sha256:fca4671ee74c6d9609f7d51b42b845d427b6b5c1d1b82536098baa923b8ef685
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2675720512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fbe86904fff81da18e2f135e0b8990e6cff534c65939fccafb40ee23bf2c5c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 15:20:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 14 Jan 2021 00:48:22 GMT
ENV MONGO_VERSION=4.4.3
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Thu, 14 Jan 2021 00:48:23 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Thu, 14 Jan 2021 00:51:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 14 Jan 2021 00:51:58 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 14 Jan 2021 00:51:59 GMT
EXPOSE 27017
# Thu, 14 Jan 2021 00:52:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f84df50d9e20cf852bfd3555d4e56feabf7b9c735e48c613fc461146876bc03`  
		Last Modified: Wed, 13 Jan 2021 18:31:55 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4571507aab07a38e1e7d473d013fe0a3b0b3a2a73696a9ff2cb17fbad5c2703`  
		Last Modified: Thu, 14 Jan 2021 01:11:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e2b8c18e7b9b79ffcc775ee51ec1c41c3478b0bedf490cce5ef381677875cd`  
		Last Modified: Thu, 14 Jan 2021 01:11:47 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a403d16dce7b5b631c252cf835c226e0adec10645da537114ab897c2f2935e7`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25a1d47e5eab05402a090b3b5a6ff42355e61ac3d5ee723fe8031a0f0dd0c3a`  
		Last Modified: Thu, 14 Jan 2021 01:12:27 GMT  
		Size: 239.9 MB (239940409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3d8191dd9f798b0e4122deb2402d16d9d406d7047777c4ad956b33b964b60d`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5c6ba724923315c456a02a532340de416b5982124d271d0f34f869e7817070`  
		Last Modified: Thu, 14 Jan 2021 01:11:44 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205a8d939284c6fbffddedbe22733df036277ff665dc7de510a782ee88fe910e`  
		Last Modified: Thu, 14 Jan 2021 01:11:45 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
