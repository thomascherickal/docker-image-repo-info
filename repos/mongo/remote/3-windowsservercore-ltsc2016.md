## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:34342e4f7e97658b03d1481ff362b12cff15d4a0e446b59bbc126b7a76bd45ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4046; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.4046; amd64

```console
$ docker pull mongo@sha256:f02bcd2f833bd4d94fa4f13dc487d9f582f5a709e09dd53a655f41429800c9aa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6465440501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa15b36695e78e5c8792509ef2ce11cb17c5d3cb2fec4b7482ea35149de813d0`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 28 Oct 2020 18:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Nov 2020 14:26:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Nov 2020 21:13:38 GMT
ENV MONGO_VERSION=3.6.20
# Wed, 11 Nov 2020 21:13:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.20-signed.msi
# Wed, 11 Nov 2020 21:13:40 GMT
ENV MONGO_DOWNLOAD_SHA256=341d1163c192488596e01219b50c14c9113ad0c305b0aef73f271d9746e44aa1
# Wed, 11 Nov 2020 21:35:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Nov 2020 21:35:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Nov 2020 21:35:49 GMT
EXPOSE 27017
# Wed, 11 Nov 2020 21:35:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4830fb08bc2df7ae80548c349b880c263ea87a7b93e13ecbc77c862b6e179558`  
		Size: 1.7 GB (1700572904 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9affba5fa493b09d48e6bd56c0d7b0eb03d1dbaa80493dd08cb18a3c9ddfbb67`  
		Last Modified: Wed, 11 Nov 2020 16:54:10 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e364635f0518ca5f9c97814abb56232be31bca4a7a5ce4ad6fc1d3e75c1d30`  
		Last Modified: Wed, 11 Nov 2020 23:42:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65964aad08ba90843076934592b6dcf6e5f1b6437f7867257c3651e73e4a1b2`  
		Last Modified: Wed, 11 Nov 2020 23:42:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009e5c9b0485ce1fa745f4c8d522a189936e5c883c965f5debef4fceb8bf12ff`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50c687076d78d080e43376e68606e03e31b492282264928005e6c7ddb909dfc`  
		Last Modified: Wed, 11 Nov 2020 23:55:51 GMT  
		Size: 694.9 MB (694873709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6aa738282ed0ef03c7c3b5ce6c93c9777db559f5cf0c6ba5d71776fb05cc1d`  
		Last Modified: Wed, 11 Nov 2020 23:42:30 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670658686972e4d435d9e324dd0d0ace6ebe050bdf8b4396614e389341e8a3e7`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab04eb4d040b80f2e25a235e1640f7e0b850f4fa2ddfe8feaed33b6a2dac3cd`  
		Last Modified: Wed, 11 Nov 2020 23:42:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
