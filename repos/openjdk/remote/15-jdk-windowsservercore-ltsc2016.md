## `openjdk:15-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:8f9d3dfc971d94a87073aad4c8c117f43d7cb3c59b6b9253778c83582dd22087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `openjdk:15-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull openjdk@sha256:d7ab153ae8f109462c27ada2387d4522dde40e34051ecb5838bed69b31b26dca
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5945987767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daa579528e5188722117a1e56a8423a7d000a732e1cbf3e9e432f151c419743c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 09 Jun 2020 22:38:24 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Tue, 09 Jun 2020 22:38:26 GMT
ENV JAVA_HOME=C:\openjdk-15
# Tue, 09 Jun 2020 22:39:49 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Fri, 26 Jun 2020 20:03:19 GMT
ENV JAVA_VERSION=15-ea+29
# Fri, 26 Jun 2020 20:03:20 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/29/GPL/openjdk-15-ea+29_windows-x64_bin.zip
# Fri, 26 Jun 2020 20:03:21 GMT
ENV JAVA_SHA256=d4db5fd712be47fb8d68ccdbc41bd5e7f3498fc4390f9554973a2023fbe155dc
# Fri, 26 Jun 2020 20:06:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 26 Jun 2020 20:06:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20399ac1a4e75ca1edbca4b2438a810ea66dbe6bdd128414ab987881b5ed641`  
		Last Modified: Tue, 09 Jun 2020 23:18:34 GMT  
		Size: 5.4 MB (5393368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e109766083929743d0ebae21d2c4462a8a05288902a46c372f19b156e917499b`  
		Last Modified: Tue, 09 Jun 2020 23:18:31 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad18636634fe84f93305aad5666d54f223ccc25d87a66f0d2093b0f233acd2d`  
		Last Modified: Tue, 09 Jun 2020 23:18:32 GMT  
		Size: 5.4 MB (5367532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c67b476fecd81eb2fe8821bb86184260794b355bfe92452905e9bbfbb649ff8`  
		Last Modified: Fri, 26 Jun 2020 20:18:08 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66956a775818a11d3167f8a40254e5db50b5e37f7ecf67a462fb61d572f48195`  
		Last Modified: Fri, 26 Jun 2020 20:18:08 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b0dab957b7888ac5556498b255910a93d8ac354619177b47ac995f74d63a20`  
		Last Modified: Fri, 26 Jun 2020 20:18:09 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c001a49fcfe52cd75e32de13d99f78551257a8f5acdee1be07fb2a2e2dadbd`  
		Last Modified: Fri, 26 Jun 2020 20:21:54 GMT  
		Size: 201.2 MB (201222237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978dd48745913aae725a6dd26613b57820428ce8b184cf763f26d948bf0fbdae`  
		Last Modified: Fri, 26 Jun 2020 20:18:08 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
