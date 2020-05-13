## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:2617684e95c344a22141b15f413f83531aaa3cb64ec8026f12e9ccd8121755fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull mongo@sha256:8559897e88ab05cfeb4962c76d0cecc55b6f6bc18568e5c4fac7f19fcfe072d5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1809779535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604f79c9e4d34313c423366a9a07c9f9c1ccc5906878a24a6f4e66a77548167e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 13:04:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 May 2020 20:33:49 GMT
ENV MONGO_VERSION=4.2.6
# Wed, 13 May 2020 20:33:50 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.6-signed.msi
# Wed, 13 May 2020 20:33:51 GMT
ENV MONGO_DOWNLOAD_SHA256=401ebc0c087058cd98194046bbd4fbee243592cf9397f36a1fafa208de4ac21e
# Wed, 13 May 2020 20:50:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 May 2020 20:50:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 May 2020 20:50:35 GMT
EXPOSE 27017
# Wed, 13 May 2020 20:50:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6e220442d94ba050201e82fee90c58b5e714748e7906735032367404c473c91c`  
		Last Modified: Wed, 13 May 2020 14:27:38 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b1ca9aacc42c443cb2e7a4017fd38cf4b8b250cf8dc87a52e543ffdaaf1126`  
		Last Modified: Wed, 13 May 2020 21:18:50 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1411594fa2436ec0ee122bc74abe4714acc98aa37f389160c03b3e255c0c594`  
		Last Modified: Wed, 13 May 2020 21:18:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f70bed59679c6c2b6b01ca8d8503bc16b4064ca7c07a9e3bc398fc4c10c56e`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5e4f133ec92be71aab42104a062fafb2d89460e3d5c6732030c064d7ad563f`  
		Last Modified: Wed, 13 May 2020 21:19:11 GMT  
		Size: 91.4 MB (91438700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf02f4642646d41fc6862e8e4bcd44a9baad5212631f319230bea71956c6180`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be6bb2028dfa7096f653e71c72c2bdd293aab4ae40eef69f96ec8474f22527f`  
		Last Modified: Wed, 13 May 2020 21:18:48 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b3b1c289018ed8728b4505f4aed2fa36dc7957bbb9b45afddafeaef210cb9d`  
		Last Modified: Wed, 13 May 2020 21:18:47 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
