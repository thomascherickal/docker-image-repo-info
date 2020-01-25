## `openjdk:15-ea-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:a10ca7075ff5d5b41b11637f483227cb183ea1501648eeedb595881a8854bf85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `openjdk:15-ea-jdk-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull openjdk@sha256:f6cf544b48e256a2bfa90f9dbe525425be725618e00f800e6ce63aebe3a06346
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2416616914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e2fe70d7add9ba68e0a70a3cb1c38fecc409f3fdacd7a9274a4308aea668f2`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jan 2020 23:47:06 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Tue, 14 Jan 2020 23:47:08 GMT
ENV JAVA_HOME=C:\openjdk-15
# Tue, 14 Jan 2020 23:47:31 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Sat, 25 Jan 2020 03:59:24 GMT
ENV JAVA_VERSION=15-ea+7
# Sat, 25 Jan 2020 03:59:25 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/7/GPL/openjdk-15-ea+7_windows-x64_bin.zip
# Sat, 25 Jan 2020 03:59:26 GMT
ENV JAVA_SHA256=43e95b54566cdc58ec11ec778a37e9563a4bb8771fcd3af4f39380ff99d7c6d0
# Sat, 25 Jan 2020 04:01:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 25 Jan 2020 04:01:52 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe8a4080f0d1077681de059bc8597064c929d967b370eac061cacf38283adfe`  
		Last Modified: Wed, 15 Jan 2020 01:45:23 GMT  
		Size: 4.5 MB (4547614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0999496898b39d56596bc2d3245e819970ebe69da77cf3fe1f27527f01cd6428`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369268aba26b31281a3faa935154fe9feaf8ee03872fea566a30dc11dafbd2e0`  
		Last Modified: Wed, 15 Jan 2020 01:45:21 GMT  
		Size: 289.6 KB (289641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1280565238ed2a973d806c79372443b1bbc44c6eadc2de52104bae603904757e`  
		Last Modified: Sat, 25 Jan 2020 04:17:19 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ae2674397fa0fe181210d9b37274c0ba2621b479825f218ece43db0353349a`  
		Last Modified: Sat, 25 Jan 2020 04:17:19 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0612717af9eb5216206aaa0e7f2fd82693049a2036ce2327a51459cd4d94badd`  
		Last Modified: Sat, 25 Jan 2020 04:17:19 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f61fc7b0bd1351be317bf71ff050ccf34c0def63cfd1f24d79f52f0f813a3c`  
		Last Modified: Sat, 25 Jan 2020 04:17:40 GMT  
		Size: 194.4 MB (194361353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43cf441378d8c7eef928721c3401a7da49ef4e627bfa66aa9efbe79b76bfed9`  
		Last Modified: Sat, 25 Jan 2020 04:17:19 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
