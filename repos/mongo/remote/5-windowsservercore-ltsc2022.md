## `mongo:5-windowsservercore-ltsc2022`

```console
$ docker pull mongo@sha256:b7d4aee3b2472bffbd0e0b3c0170a284a140741552ebdf77929e309be82ac3c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `mongo:5-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull mongo@sha256:35f752f7ed55e3f211356e3433988121bcdc2ac42995a108a8cf9b8c70b5e7ef
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2173723945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:681fa2e8f10106f7c6f0186b1cce9f2a3cbd3a108260f0c213db058f3bc6e80a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 02:54:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 26 Oct 2023 23:24:01 GMT
ENV MONGO_VERSION=5.0.22
# Thu, 26 Oct 2023 23:24:02 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-5.0.22-signed.msi
# Thu, 26 Oct 2023 23:24:03 GMT
ENV MONGO_DOWNLOAD_SHA256=ce6c6b3365e23ffc2245dce2030523ef4440fd154b6965ac5d4e19bc86e86a4d
# Thu, 26 Oct 2023 23:25:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongod.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 26 Oct 2023 23:25:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 26 Oct 2023 23:25:20 GMT
EXPOSE 27017
# Thu, 26 Oct 2023 23:25:21 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c131d94d08cb023367d3fd8434c336e9d07495660367cc521ddff869fb44dc7d`  
		Last Modified: Wed, 11 Oct 2023 05:52:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9302846933847cc653f44a6a6e40ef6d4e430ad3e5e2b506d9a49e17b0f43c10`  
		Last Modified: Thu, 26 Oct 2023 23:37:09 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0abf471f5c9a8a2e07099b64cdd4f8e428517c42da4e4efa6b053916a68d40`  
		Last Modified: Thu, 26 Oct 2023 23:37:09 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422b5f43598f36108a26e372bd688de1785eda2919622f522d66baa3de0dbd07`  
		Last Modified: Thu, 26 Oct 2023 23:37:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b28be575219fa6815734fda18c0bba69a5129483f9e2e82e3d0c2aca4c46e25`  
		Last Modified: Thu, 26 Oct 2023 23:37:53 GMT  
		Size: 313.9 MB (313870937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2dbe65c636ae8a920715f8456066688eb705027e21db83afc578e5305d022ba`  
		Last Modified: Thu, 26 Oct 2023 23:37:07 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede4a520018604c0652390dd1dc7b5278ca6a46dc4cb0bf5c8ae9d8a31c253b4`  
		Last Modified: Thu, 26 Oct 2023 23:37:07 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3592402f474245e269651ea6ee3350933a279a4ee370f9166f7cd4a1118737d`  
		Last Modified: Thu, 26 Oct 2023 23:37:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
