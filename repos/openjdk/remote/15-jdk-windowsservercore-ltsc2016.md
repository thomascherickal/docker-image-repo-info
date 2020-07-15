## `openjdk:15-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:18ddf828364bfaacf40862d618843313daf0a32be7ff546255d9090e1e1d719f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `openjdk:15-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull openjdk@sha256:b160f33ba9a5848671aaabaa9f73b35ed87b303333b9a45200699c95df94c57d
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5953791965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18fafdf13ffbf152a09f6019e82fa960586111de7594bc779666f4587ca91f83`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 01:50:16 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 15 Jul 2020 01:59:06 GMT
ENV JAVA_HOME=C:\openjdk-15
# Wed, 15 Jul 2020 02:00:32 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 15 Jul 2020 02:00:33 GMT
ENV JAVA_VERSION=15-ea+31
# Wed, 15 Jul 2020 02:00:34 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/31/GPL/openjdk-15-ea+31_windows-x64_bin.zip
# Wed, 15 Jul 2020 02:00:36 GMT
ENV JAVA_SHA256=0a97cdf251e6da9f867ba2699332735ce271048bf3213c9355ef078a991d2310
# Wed, 15 Jul 2020 02:03:21 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 02:03:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccabcd61311861039196ce34ec8b8b74f236a3b135a888ca230811c6f8a439bc`  
		Last Modified: Wed, 15 Jul 2020 02:43:13 GMT  
		Size: 9.9 MB (9852381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08489b93b58decf5c8556b628a7efab4affaeab05bbbce6dbd37befa0717d5b0`  
		Last Modified: Wed, 15 Jul 2020 02:45:37 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1523ffb63a480bebab9060b8dcd04922c340b99d6a3dfe0168eef164a279333`  
		Last Modified: Wed, 15 Jul 2020 02:45:38 GMT  
		Size: 5.3 MB (5336634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b9b035c0a658d3b2743708f81da01872580f66b04e6ac59861d4306ac23bb0`  
		Last Modified: Wed, 15 Jul 2020 02:45:34 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb3b911dab9f9f5187a69761613c39b8ecd1538195e6f2fa2731ba2fa0cf421`  
		Last Modified: Wed, 15 Jul 2020 02:45:33 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad2d6515ee7908fec15ba18694cd5d70657c8cfc78fc46b6f85314d4a57d056`  
		Last Modified: Wed, 15 Jul 2020 02:45:34 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18c98659f3667e3d11322609eee2c0d70bee4305f35a1be61e215efeb7c9c56`  
		Last Modified: Wed, 15 Jul 2020 02:45:56 GMT  
		Size: 201.1 MB (201133944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd252fe63eba874ed134a852903d60b95c1744ed4e497321ff621d7258b76e5a`  
		Last Modified: Wed, 15 Jul 2020 02:45:33 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
