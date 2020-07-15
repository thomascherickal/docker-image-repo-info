## `openjdk:16-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:7dbf35ebd9a62766255ba43eb2b366f674794514c2529115ab2f8f4bbbd04be2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `openjdk:16-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull openjdk@sha256:1a59f09807cacbc1781f2b894b2d8d43da938f348c487e0edda359f04ff595c5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5954447110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784dd2fe30d72ad574d70ae4c33090cfe44a1f6f17e04f9bbda56fe5dca81cb8`
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
# Wed, 15 Jul 2020 01:50:18 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 15 Jul 2020 01:51:44 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 15 Jul 2020 01:51:45 GMT
ENV JAVA_VERSION=16-ea+5
# Wed, 15 Jul 2020 01:51:46 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/5/GPL/openjdk-16-ea+5_windows-x64_bin.zip
# Wed, 15 Jul 2020 01:51:47 GMT
ENV JAVA_SHA256=35d6b27ea5cc47f5caad0171e0a6bd120277c572c30c4e0d83d19ef63b74bc4a
# Wed, 15 Jul 2020 01:54:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 01:54:34 GMT
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
	-	`sha256:bfe0ef8e7d2128d8c84e3f4ee9aa336c9283b3593612b51d5064c853e7b29678`  
		Last Modified: Wed, 15 Jul 2020 02:43:08 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452c9dc43f44e3a09fe36211818cb5063135234cfea03935d12c62801b50888c`  
		Last Modified: Wed, 15 Jul 2020 02:43:10 GMT  
		Size: 5.3 MB (5333218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f08f97065c8c81b23d4d61b0be3d07d9efb88f01334b79d01f244eb141f360`  
		Last Modified: Wed, 15 Jul 2020 02:43:06 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c848d527d8ae5bbc2b0fa70e4a6b2df1aa7a5f4aa96c354631a35849dbfb2912`  
		Last Modified: Wed, 15 Jul 2020 02:43:06 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e6073e9474745744d68001f099891d441c3a8c0cfa27c94e27cf25c0848ead`  
		Last Modified: Wed, 15 Jul 2020 02:43:06 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568a510e3755c6b34f439afcdd4aa36642d3f8fa4b3811343ffa55e39c41ba97`  
		Last Modified: Wed, 15 Jul 2020 02:43:31 GMT  
		Size: 201.8 MB (201792534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e0c4a097b6659c3e1958ca7f57d7643a5b12056d7fee076019e8ec50dd8460`  
		Last Modified: Wed, 15 Jul 2020 02:43:06 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
