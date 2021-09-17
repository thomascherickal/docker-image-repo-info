## `openjdk:18-ea-jdk-windowsservercore`

```console
$ docker pull openjdk@sha256:52ad12ae0f10191216748c15c9a9b23d3aff60bfb6a064c9a1506dc65cd278e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `openjdk:18-ea-jdk-windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull openjdk@sha256:1112c819ea92a5c8711972d9a134be96af43eca1698ce7fdc3df20472a1cf459
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2870597033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3375b7865a792b730534d45eaa98741013fbeffbb46473261b552c0e923234bd`
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
# Fri, 17 Sep 2021 19:30:09 GMT
ENV JAVA_VERSION=18-ea+15
# Fri, 17 Sep 2021 19:30:10 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/15/GPL/openjdk-18-ea+15_windows-x64_bin.zip
# Fri, 17 Sep 2021 19:30:11 GMT
ENV JAVA_SHA256=bd0121a79be31881084e84d41a16f8be15692ab5dd4cd4736d9bd7d67700dc75
# Fri, 17 Sep 2021 19:31:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 17 Sep 2021 19:31:37 GMT
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
	-	`sha256:d473cb01baa25a33aa8f544b8c08bd819d1d5ed8b8377c3d3c11d906dbb10cd6`  
		Last Modified: Fri, 17 Sep 2021 19:38:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f353ebb6ee208eb47847b1252f8769deb8d60843afbe5ca4d1a8d46c973d9c`  
		Last Modified: Fri, 17 Sep 2021 19:38:16 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a04af8ed76e491e52ac321e732807acc483be5b6530d350282531d8aff82385`  
		Last Modified: Fri, 17 Sep 2021 19:38:16 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c9ee3157fef0eb6a0657eef536dc505b99ea8403b8b7b3f448be18f2785fa5`  
		Last Modified: Fri, 17 Sep 2021 19:41:30 GMT  
		Size: 183.2 MB (183218678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab92e402c722bed6fd649b37359ef88cb5be5d8401ee249e71b6a115df9f1fc`  
		Last Modified: Fri, 17 Sep 2021 19:38:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk-windowsservercore` - windows version 10.0.14393.4651; amd64

```console
$ docker pull openjdk@sha256:5e5504eb78653397c3a31af7b8e19191c6149f2090b26d5c7df9f1d79095dcfa
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6455238682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e365d877ab8c63f988e14c7337dc58303ed9b1e72fe6ba85383a6631512113`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 00:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 00:35:51 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 15 Sep 2021 00:35:52 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 15 Sep 2021 00:36:45 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 17 Sep 2021 19:31:49 GMT
ENV JAVA_VERSION=18-ea+15
# Fri, 17 Sep 2021 19:31:50 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/15/GPL/openjdk-18-ea+15_windows-x64_bin.zip
# Fri, 17 Sep 2021 19:31:51 GMT
ENV JAVA_SHA256=bd0121a79be31881084e84d41a16f8be15692ab5dd4cd4736d9bd7d67700dc75
# Fri, 17 Sep 2021 19:33:21 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 17 Sep 2021 19:33:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8721f004192f15fe71b8626ef3f3e34cbf2cfe1d15a63b6b544ab946162ef707`  
		Last Modified: Wed, 15 Sep 2021 01:10:18 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b794d0a07a41196dae8678e4ecbb9a5766d6db31f9729bfe3f1d83963af3e0`  
		Last Modified: Wed, 15 Sep 2021 01:10:18 GMT  
		Size: 339.2 KB (339172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d3bfbbd6119f5d4c8cdfa80560f7d1dfa6730c4d5af995fee76f3decd44528`  
		Last Modified: Wed, 15 Sep 2021 01:10:17 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8da815f1cb98dfe565a92045b7ed382138e2c7bbbba2982c14bcecce8161396`  
		Last Modified: Wed, 15 Sep 2021 01:10:17 GMT  
		Size: 335.9 KB (335946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d0441b64bfd162e0c790e69d86f0f948208d5cc86f2d3c6231c4d1198f5885`  
		Last Modified: Fri, 17 Sep 2021 19:41:55 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26a1fa87f3a557d52f2956bc69ea2e560e5029d43a9fe7c152cbaef0de8eebe`  
		Last Modified: Fri, 17 Sep 2021 19:41:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782165ac1acea3e41b26f75000618203211f45a3721b8779e27ffc919891a513`  
		Last Modified: Fri, 17 Sep 2021 19:41:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2de87d84b52034c7d605db8f9c2f852a148379950e89e4b0314a66319e516f6`  
		Last Modified: Fri, 17 Sep 2021 19:42:13 GMT  
		Size: 183.2 MB (183227044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01f3702ad5a86965aa3621c22b9b02e4685106d80c8344fdf7443dac76f4be6`  
		Last Modified: Fri, 17 Sep 2021 19:41:56 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
