## `openjdk:17-ea-25-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:16086d37e1f6927922632118093b5e9411313a3fba3ce7c33f95237cc2ddfe67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `openjdk:17-ea-25-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull openjdk@sha256:8b31f84af8c175e9d3658c0c28c6468ec22390c7db30f993c66129aa50378b8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6447667694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b827df457af0fa60b1b9f181d778117ff54ccda4985d8e34d13ebacc58be81e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 16:48:43 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 09 Jun 2021 16:48:45 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 09 Jun 2021 16:50:13 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 09 Jun 2021 16:50:15 GMT
ENV JAVA_VERSION=17-ea+25
# Wed, 09 Jun 2021 16:50:18 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/25/GPL/openjdk-17-ea+25_windows-x64_bin.zip
# Wed, 09 Jun 2021 16:50:20 GMT
ENV JAVA_SHA256=b1cf7a899b6687db3553770a0ec1a6e17c5c357d44d2bf0c5845251c32e2d659
# Wed, 09 Jun 2021 16:52:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 09 Jun 2021 16:52:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030344af2a85aa48f4c1eb2866fe22830344ab5752d72cb3dec80e7234b68523`  
		Last Modified: Wed, 09 Jun 2021 17:24:45 GMT  
		Size: 343.9 KB (343868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41cbdbabbc3dc8df16e40d2439f3f57faa24b3d6cfde3f6407dd05c7dc09845`  
		Last Modified: Wed, 09 Jun 2021 17:24:44 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5c2af984d599f4fe5db096a3ad4bc6ea4d953344734d21db1d9a3a3b2ce0b2`  
		Last Modified: Wed, 09 Jun 2021 17:24:44 GMT  
		Size: 295.5 KB (295512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c141f67c3727faa8ce8fac874734b3807b70d627edc5099f7d54328483a78967`  
		Last Modified: Wed, 09 Jun 2021 17:24:41 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e156573947ac7c71c10298be0da68b4505b3f35ebe9866c96f2fa56a56857bde`  
		Last Modified: Wed, 09 Jun 2021 17:24:41 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7757116dda57dcc4015745f0f48caaf9ab0d4f155a1980bc0d7b62e062a37697`  
		Last Modified: Wed, 09 Jun 2021 17:24:41 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d7ebf92b08c615e04232da9dbcd369cd8cc3b2f2974847a2444fe1527ea604`  
		Last Modified: Wed, 09 Jun 2021 17:25:02 GMT  
		Size: 181.3 MB (181292539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986127fa0d087a01baeabd687e15537b0771e5a4d47e3447fdf6b38e00810028`  
		Last Modified: Wed, 09 Jun 2021 17:24:41 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
