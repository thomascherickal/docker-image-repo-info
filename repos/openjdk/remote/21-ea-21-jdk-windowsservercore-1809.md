## `openjdk:21-ea-21-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:710fca8f5d4247d2d4fed4830adecc3806607c549292eae8dbd76e439ebf4fd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `openjdk:21-ea-21-jdk-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull openjdk@sha256:d7fe4cb566012eeb83bd52f2d07eae3c21800f1f8c335964747c8cd1004bd859
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2269001981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e1f3ff2b2bfd8cd17f5fe6b6a5863ab90dab9eb149ac11024eef75ea96e506`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Apr 2023 23:42:24 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Tue, 11 Apr 2023 23:42:25 GMT
ENV JAVA_HOME=C:\openjdk-21
# Tue, 11 Apr 2023 23:43:30 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 04 May 2023 23:16:21 GMT
ENV JAVA_VERSION=21-ea+21
# Thu, 04 May 2023 23:16:22 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_windows-x64_bin.zip
# Thu, 04 May 2023 23:16:23 GMT
ENV JAVA_SHA256=956977cb5020e6f7b75a2e06336cf858b8b131d6a57f9b0ca0b7f9b62b4e82be
# Thu, 04 May 2023 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 04 May 2023 23:17:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2a17e347e3144ab020e098f925bc273e89f499e03114bea80260a0bc601f9c`  
		Last Modified: Wed, 12 Apr 2023 00:50:56 GMT  
		Size: 487.7 KB (487655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c03d658bc6a61ee9591db424ef2db8137173e1ff03e628327eda8134490cb46`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4c3c308ea664c1238fc40d20ade9c94a79f29169edf764c414e542fc4495ab`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 311.4 KB (311449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3351505e6a69cda24e848337bf3567ef927fb4dff19318139c89a52ce02e94f`  
		Last Modified: Thu, 04 May 2023 23:19:53 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6194913e91ca0cfac1783e6915894a2c82bf7fb4bb9b4752bd007669b2e89a6d`  
		Last Modified: Thu, 04 May 2023 23:19:53 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc488a509d307bd05b619b43434e3cdab85f3fc7d88c8ed104582562e73bc247`  
		Last Modified: Thu, 04 May 2023 23:19:53 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e585f8cd55e4b199edacf3b0ee01a69934f722cba9831095fe1078c1605ad6f`  
		Last Modified: Thu, 04 May 2023 23:20:11 GMT  
		Size: 196.9 MB (196903156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b82c3701695fc09a5ef948215b06a82f8425117e9fdf7dedae23ce1caef2793`  
		Last Modified: Thu, 04 May 2023 23:19:53 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
