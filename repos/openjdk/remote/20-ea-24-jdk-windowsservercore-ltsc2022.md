## `openjdk:20-ea-24-jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:0d656991a468ae3a00e5bfe54bbec074412932337d94c5f821bc4ab4cd38ba14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `openjdk:20-ea-24-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.1249; amd64

```console
$ docker pull openjdk@sha256:1450357f57dd7444b6c87d62d0992200fc9eeec451323220cd821af03b5310be
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2676783890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e6ad0d151705d05a83c429d49337c5f297889d40bd21f162eaf464d4efeb7d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 17:20:09 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 09 Nov 2022 17:20:10 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 09 Nov 2022 17:20:37 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 18 Nov 2022 01:14:24 GMT
ENV JAVA_VERSION=20-ea+24
# Fri, 18 Nov 2022 01:14:25 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_windows-x64_bin.zip
# Fri, 18 Nov 2022 01:14:26 GMT
ENV JAVA_SHA256=d8045699c2776b155e5266733e02de5568443d48218d346b5c8f648b915038da
# Fri, 18 Nov 2022 01:15:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 18 Nov 2022 01:15:31 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f5ce72a05e01b629001eb0ff2b493ddf6cd8e3c7a836607dc83cfbbec299b3`  
		Last Modified: Wed, 09 Nov 2022 17:35:31 GMT  
		Size: 614.7 KB (614677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766f89a2f9cf276bf435dc9be37e180dfcfc54b750ca8cca41b1e0673eb95abe`  
		Last Modified: Wed, 09 Nov 2022 17:35:30 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3329d7d902a4cde0c4f3848690267bd771e713ccee926c04fc723e62ad0105e8`  
		Last Modified: Wed, 09 Nov 2022 17:35:31 GMT  
		Size: 546.1 KB (546089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c958d24e5cbb7227468de5ba75546bf89af8b680f26609a70f9af1fc740f89`  
		Last Modified: Fri, 18 Nov 2022 01:20:50 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ee11a639d1f03905f593e07c56ec14db5ae44b952b5a7edcd1ceee220e64ef`  
		Last Modified: Fri, 18 Nov 2022 01:20:50 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a36bb205d66f1b13493b2cc58e794b0a2a8ee59ede1c8407e8d4ace773e7234`  
		Last Modified: Fri, 18 Nov 2022 01:20:50 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fac7bad25cea0ebacc0367ef7bdb48b922a65623725fe698d7806b3f325a7dd`  
		Last Modified: Fri, 18 Nov 2022 01:21:11 GMT  
		Size: 193.8 MB (193845954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d66315068f5973532163b90779e9597f6395cfdd5e70bdd37595b1c5f683e25`  
		Last Modified: Fri, 18 Nov 2022 01:20:50 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
