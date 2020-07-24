## `openjdk:16-ea-7-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:bc822a369cf0ded67c9a0345a8669b338357239a4c3fb0b55ec1e9a970f06563
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:16-ea-7-jdk-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:bb5f6f1f8e2b9693391feea7ad9b2b09e5ed1b0290ff277b454764beba81d611
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2516366028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f96d481a2293b55dad0a416bf10a59949151e506d345091e6a6c7e878788079`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 24 Jul 2020 18:15:15 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Fri, 24 Jul 2020 18:15:17 GMT
ENV JAVA_HOME=C:\openjdk-16
# Fri, 24 Jul 2020 18:15:38 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Fri, 24 Jul 2020 18:15:39 GMT
ENV JAVA_VERSION=16-ea+7
# Fri, 24 Jul 2020 18:15:40 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/7/GPL/openjdk-16-ea+7_windows-x64_bin.zip
# Fri, 24 Jul 2020 18:15:41 GMT
ENV JAVA_SHA256=51f0d39c14feb7c4ce970aebb3ec35c33b6511023842c1122c62b83ea3292339
# Fri, 24 Jul 2020 18:17:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 24 Jul 2020 18:17:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ded26bb196400f1cf541826f3f44c1025664089ba3c58aaf3b7afca018655df`  
		Last Modified: Fri, 24 Jul 2020 18:33:13 GMT  
		Size: 9.2 MB (9158926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5331aed97b004095fa939fcf32a60be450a462a6f710beea77b4507e4416fe`  
		Last Modified: Fri, 24 Jul 2020 18:33:10 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a58fddb23ea3a144374036b7f928eae28c094b087ba205a4baf4682fa25526`  
		Last Modified: Fri, 24 Jul 2020 18:33:10 GMT  
		Size: 314.1 KB (314142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040d8e7b6bbcaa8fe9decd8506d9d718e274845544a74b772200554dfc06d565`  
		Last Modified: Fri, 24 Jul 2020 18:33:07 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0606679a8e3060ab4af4a10762769adf8af071ea395181b2d9820bb0b602e4`  
		Last Modified: Fri, 24 Jul 2020 18:33:07 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27af739d03a2f327b178e8c6da27e7051f82c658357e89798db52b9d479af9b0`  
		Last Modified: Fri, 24 Jul 2020 18:33:07 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d96a6c98c2dbd145a41141ac99be14e691f993eb1e4dc1df1cc626333ab379`  
		Last Modified: Fri, 24 Jul 2020 18:33:31 GMT  
		Size: 196.7 MB (196694057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41bd10864cf9bf90fcd0a495337be90cb439d9ebcdcbcc15cca4e4e49bc7167f`  
		Last Modified: Fri, 24 Jul 2020 18:33:07 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
