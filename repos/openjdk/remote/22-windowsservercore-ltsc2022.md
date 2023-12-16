## `openjdk:22-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:3e91de13e0463b203227b5006f479f25f3b85d9128341e69e5b51c658731836d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `openjdk:22-windowsservercore-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull openjdk@sha256:5108e37312d8d57b1f367490d761c259096631f4308a06631a0abd85b90d64fe
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087855688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38f81ffe6720ddeb44b3308efa22acba5abbe0826dfec9159e42f9456ff30d0e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Fri, 15 Dec 2023 22:14:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 15 Dec 2023 22:14:16 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:14:17 GMT
ENV JAVA_HOME=C:\openjdk-22
# Fri, 15 Dec 2023 22:14:22 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:14:23 GMT
ENV JAVA_VERSION=22-ea+27
# Fri, 15 Dec 2023 22:14:24 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/27/GPL/openjdk-22-ea+27_windows-x64_bin.zip
# Fri, 15 Dec 2023 22:14:25 GMT
ENV JAVA_SHA256=522347f78607019a5c2d2478846c2ca0715ee700a7db3f78aff024e9935b1091
# Fri, 15 Dec 2023 22:15:16 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:15:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7839fc47f6e056f9e09a214230f8b7115e69419dbc74acbbb1ad6bc0caa28862`  
		Last Modified: Tue, 12 Dec 2023 18:27:40 GMT  
		Size: 500.7 MB (500674814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469eae946945ee926852d89bdb55b3ff7c8fb84a8255432d184b1dca3c42ddae`  
		Last Modified: Fri, 15 Dec 2023 22:15:21 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a58e72de81796b9c7ccdfa55ca9e400dec7c20f216ba3b941bcaf673301a854`  
		Last Modified: Fri, 15 Dec 2023 22:15:21 GMT  
		Size: 504.1 KB (504050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ace084ec98d59e05cd39afdd8b0e5018c624ad6c1770afdd6d21259bc0eb89b`  
		Last Modified: Fri, 15 Dec 2023 22:15:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0969a116040f91ebab6e6be3237a287dee8db52d38187eced24f1d88ca789b`  
		Last Modified: Fri, 15 Dec 2023 22:15:21 GMT  
		Size: 356.0 KB (356043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a44fb5cb11c659b0e000e66fa7ef41a671a07932d6a18366dd6f128fce99c2f`  
		Last Modified: Fri, 15 Dec 2023 22:15:20 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9605a9702c25dd3c072a4d8ee07388f8cda99f4b46ff062c68db61d7d754b56`  
		Last Modified: Fri, 15 Dec 2023 22:15:20 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20858b9539a907011e3efb53da83b3da5f379128731585ed478cd982030d744e`  
		Last Modified: Fri, 15 Dec 2023 22:15:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbba622edc2ed253bea3da11fef94117ee80e630b1092458fc5b44f26e645597`  
		Last Modified: Fri, 15 Dec 2023 22:15:32 GMT  
		Size: 197.7 MB (197714102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a10b1c0daec01c30d65bf5578997d41bb7445f1927c725cfe2b326c69ae0b6f`  
		Last Modified: Fri, 15 Dec 2023 22:15:20 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
