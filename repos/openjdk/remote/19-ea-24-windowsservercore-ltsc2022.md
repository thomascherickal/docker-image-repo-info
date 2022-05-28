## `openjdk:19-ea-24-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:0d166e6b542080b52e09e9deddebd024083be6b1ab7297fd63aa7dab931c0208
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `openjdk:19-ea-24-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull openjdk@sha256:038c4796fc69e44e7fd0387562690f27fd491b036e2f7ebaeffdc2471db383c2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2429906530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e880466e40de16e074b02f3ac3a7ad45b958f73469ce674ea2d39a0237e735b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 15:28:55 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 11 May 2022 15:28:56 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 11 May 2022 15:29:16 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 28 May 2022 01:15:33 GMT
ENV JAVA_VERSION=19-ea+24
# Sat, 28 May 2022 01:15:34 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/24/GPL/openjdk-19-ea+24_windows-x64_bin.zip
# Sat, 28 May 2022 01:15:35 GMT
ENV JAVA_SHA256=a5974510346929cb26c24ef0692ba91026c4e94a917c27063150b937e4696067
# Sat, 28 May 2022 01:16:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 28 May 2022 01:16:34 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7320671bb1ef07c493563d61e332d907b7a248c0d182698a877d84e65327b614`  
		Last Modified: Wed, 11 May 2022 15:56:04 GMT  
		Size: 607.9 KB (607907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c59d468f4140dfeb9ca7cccc1a19de4b9dee810da486843372bc823daddb570`  
		Last Modified: Wed, 11 May 2022 15:56:03 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613b2526877fb3edad53c027ade0fb2feb1ec41cfe4a7bfc4d5d1db891b391e5`  
		Last Modified: Wed, 11 May 2022 15:56:04 GMT  
		Size: 539.4 KB (539446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ebe123eb91fda430825bfecee39f73de2b8d60f3d4fd9e47844dc94af24d8a6`  
		Last Modified: Sat, 28 May 2022 01:23:37 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd62f6f84aa36d5d8a8c3d6b614c954e8ad62117be9f53373bcb317a52af71c8`  
		Last Modified: Sat, 28 May 2022 01:23:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c8873fcb601ea34788d96749f54b15dcd000a0b6685adbbaa8316c504f86b`  
		Last Modified: Sat, 28 May 2022 01:23:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29cb3aa465455f62fa4fa3168e9a4e3613b71ad5c20489ff943ea86d8044b3f7`  
		Last Modified: Sat, 28 May 2022 01:23:59 GMT  
		Size: 191.2 MB (191215464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a93440cc3a58a7d6293dc44186cc42ee97d68d032260d983470f973f07e1d28`  
		Last Modified: Sat, 28 May 2022 01:23:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
