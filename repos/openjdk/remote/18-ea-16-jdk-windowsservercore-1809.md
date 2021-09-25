## `openjdk:18-ea-16-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:617cff881771627b98765ec73028d6aec94ec2d25c31aa1456284bede2443771
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `openjdk:18-ea-16-jdk-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull openjdk@sha256:9d7f37632652deaa9bac26a1b066a45a16421c3ac3da975c885f1fa30aa9b65a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2870764433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436805fd0e138516d04049c21d492f1486b99554b7d434e589b4bdfe76c64289`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 00:31:34 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 15 Sep 2021 00:31:35 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 15 Sep 2021 00:32:58 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 25 Sep 2021 00:15:15 GMT
ENV JAVA_VERSION=18-ea+16
# Sat, 25 Sep 2021 00:15:16 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_windows-x64_bin.zip
# Sat, 25 Sep 2021 00:15:17 GMT
ENV JAVA_SHA256=d59e49abb435e202744d954994789e87302a9bed870f889241a5774d4ef6db31
# Sat, 25 Sep 2021 00:16:48 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 25 Sep 2021 00:16:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d714779fd458636d1b2289ae98777c0c8707a28708bffccab0b1314b59d77c`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 356.1 KB (356133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff34aee5a2ca310095a4e04d975fc389917040f43df1b7ab33cefa990b2f5794`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2a30bd406da0ac5e18d582ad2ebdb0eb00497ff4ace8dc69f07433cb6d5728`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 315.8 KB (315799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1b27d5fcdf842b0667947072ef856d28f307dca76f0f7da763ad0b389b011d`  
		Last Modified: Sat, 25 Sep 2021 00:24:26 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c98c9b1ef7a3c5463ba780adec14b6f6ae8cd00562ce25c2aefa357ddd5a2bc`  
		Last Modified: Sat, 25 Sep 2021 00:24:25 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c51a0c55974b551025b166daac5ec5818b78ccef5f55ed11b91a59d8a65c28`  
		Last Modified: Sat, 25 Sep 2021 00:24:26 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a835bbd63bd8a485ec4bc2722aa5a5e9c2c6a6466c78f7ccb251ae83345772c`  
		Last Modified: Sat, 25 Sep 2021 00:27:46 GMT  
		Size: 183.4 MB (183386112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0465b080f80a83eda9ca1a909954423499467e2f97725d16dd6031e22f11de`  
		Last Modified: Sat, 25 Sep 2021 00:24:25 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
