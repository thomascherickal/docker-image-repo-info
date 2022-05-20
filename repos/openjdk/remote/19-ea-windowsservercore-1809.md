## `openjdk:19-ea-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:051582fd99b8a4b9d5763cba96dfdb365b950b1570664e37501a8cc88649b790
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `openjdk:19-ea-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull openjdk@sha256:3da1c5ef3f1c95ebfd02016a76ea6df85f7086fbd44c6107e6ea6b414c8d41e8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2695848113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34af049aaf1d6062ee3cec60e1507f8b6bd29b2bfbd2d9eef9ce3866a24f4dbf`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 15:31:20 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 11 May 2022 15:31:21 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 11 May 2022 15:32:04 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 20 May 2022 21:16:52 GMT
ENV JAVA_VERSION=19-ea+23
# Fri, 20 May 2022 21:16:53 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/23/GPL/openjdk-19-ea+23_windows-x64_bin.zip
# Fri, 20 May 2022 21:16:55 GMT
ENV JAVA_SHA256=d86c8cd64a8563ff063cc3b7e2fadcbee2e96066cc1a443397ae01274bc8300d
# Fri, 20 May 2022 21:18:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 20 May 2022 21:18:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d16e9483c31353bee635610112700e2b9f38d45e154c79f5331ff07164b3f07`  
		Last Modified: Wed, 11 May 2022 15:56:46 GMT  
		Size: 488.1 KB (488114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3edb7b7391c69a83de5498a0df582da9d86d3dd21d40664b920bc4c45a896b`  
		Last Modified: Wed, 11 May 2022 15:56:45 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009f37a60cc36209d3b0aac27db2934d6ddfb285c5845c2dd7227945d3aff595`  
		Last Modified: Wed, 11 May 2022 15:56:46 GMT  
		Size: 317.1 KB (317078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02c30ff0eb1fe7eaf191b15083a52f9137a8a0dfdfc00f37577358959393311`  
		Last Modified: Fri, 20 May 2022 21:27:51 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ce4db62756cb2c41a7feb0db30baf82dec67e13f2bc377c72cdd580df2367f`  
		Last Modified: Fri, 20 May 2022 21:27:51 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcec332f6cd0cabac90745237caa1419b25071cb8210c34e285154617e01beca`  
		Last Modified: Fri, 20 May 2022 21:27:51 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49786fa9afceb66ae3d2bb5d361a44a0f504aeb79c2f3ac964261e174af79943`  
		Last Modified: Fri, 20 May 2022 21:28:13 GMT  
		Size: 191.0 MB (190978606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825a6a9114084a46673b4af350713a71c42998b47506ecd7ef111a57662eb355`  
		Last Modified: Fri, 20 May 2022 21:27:51 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
