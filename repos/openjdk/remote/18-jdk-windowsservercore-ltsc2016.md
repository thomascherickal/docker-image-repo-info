## `openjdk:18-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:14c007c63bf8ea483cec3ee1675b71fe980e63c3f74679b05f71e76eea00c27d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `openjdk:18-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull openjdk@sha256:fb2a58841fb7ca0136323c8850f56d05f4cd7fdaf68e1e951ca092cf2baf77ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6454583464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dee5ddb369796b89806f511e8fa95a776373a44e3c29f1e1d32eff875faf01e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 17:26:21 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 11 Aug 2021 17:26:23 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 11 Aug 2021 17:27:57 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 11 Aug 2021 17:28:00 GMT
ENV JAVA_VERSION=18-ea+9
# Wed, 11 Aug 2021 17:28:03 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/9/GPL/openjdk-18-ea+9_windows-x64_bin.zip
# Wed, 11 Aug 2021 17:28:06 GMT
ENV JAVA_SHA256=a0af7b8be120ff46eec1522875be7e969d43fbee1e06a535ad835f4a57e619d0
# Wed, 11 Aug 2021 17:30:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 17:30:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85818d8ae526f813cf82bc85044b12bcf64737f7bce6c6b2d983a6db1251a488`  
		Last Modified: Wed, 11 Aug 2021 18:20:44 GMT  
		Size: 348.4 KB (348421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97555b86e64e63a554a03c6f11081f8cbdf6c342fcc22e636805874c5bc3621`  
		Last Modified: Wed, 11 Aug 2021 18:20:44 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170015a5368a4254730393e471c1266819b31109af34e6a507a6ba90f74c3bdf`  
		Last Modified: Wed, 11 Aug 2021 18:20:44 GMT  
		Size: 300.6 KB (300628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1def6e5ed29866ae7005b216d7bdcf35cdb542a041773557fc02b72c211796`  
		Last Modified: Wed, 11 Aug 2021 18:20:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e5b74be33e253ed85cc913f1209edce211cff6af9492a8ea5c268316735629`  
		Last Modified: Wed, 11 Aug 2021 18:20:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cfdb435cd0cc40cd79e4b1a5331f51f972b696263f1751d6ea40cb39e08ff9`  
		Last Modified: Wed, 11 Aug 2021 18:20:40 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e93d7b12eefaff73108e1e3abc96bec317955390fd78a38972a6b6e8b55b98`  
		Last Modified: Wed, 11 Aug 2021 18:21:02 GMT  
		Size: 183.0 MB (182959865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bd9aaf6172c5f76f2a8799f6350ad17c54b9fa6d8d211ed73ff84d64bb6cbb`  
		Last Modified: Wed, 11 Aug 2021 18:20:41 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
