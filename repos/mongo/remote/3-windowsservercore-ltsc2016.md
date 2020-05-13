## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:06b77b67cd90a2df18d51fb4e66b0ac8b8b044d1f6993bc2eac6efdaa80d8d37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull mongo@sha256:acd783dbf688421006292e9842b432a2b78cbcaf91c745bcd49370ae47026421
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187746906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b55328b36a87aa58328bb2e91ff24e529cdd348a890894df7cb40531fb0fef84`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 13:13:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 18:58:18 GMT
ENV MONGO_VERSION=3.6.18
# Wed, 13 May 2020 18:58:19 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.18-signed.msi
# Wed, 13 May 2020 18:58:20 GMT
ENV MONGO_DOWNLOAD_SHA256=d6a17f96adcda714f523a4b119419b8bf93269542acee70e2b5e899d6d93efdc
# Wed, 13 May 2020 19:15:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 19:15:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 19:15:12 GMT
EXPOSE 27017
# Wed, 13 May 2020 19:15:13 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d9ecf24b3b7ef3e61c8b38d40e28e57a80552d6c97884f4cc142af2110ddff`  
		Last Modified: Wed, 13 May 2020 14:28:09 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61a165cbd6bea351efe1d4d3cc43dba0e0d85306b619be5112ad55bb6150747`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48a0a7b87b33d9ca3f2b8f406f109f45ad163d789fa153ab55e2635375f7771`  
		Last Modified: Wed, 13 May 2020 20:51:33 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc000ddbe32e263669cf5e94f347c8bbddde8ba681e710d9348a30cd07e89e`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26afe47326c981410c152967eb7bfe9f48d4f15df1112f18cff72e54c2d30be`  
		Last Modified: Wed, 13 May 2020 20:59:16 GMT  
		Size: 455.8 MB (455849206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66ddb93b85a732d1f255dcc815997332251e1e8a484ad6797041e883f017bf7`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59dee24b645cca9e056821ed6e61c8aa8446abc03dd43cda9e0e58c278b6a1a`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c03dc16f6492a0cc3b36c10181e6f9aab335f607fc59cdf52816cbab7b05a37`  
		Last Modified: Wed, 13 May 2020 20:51:31 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
