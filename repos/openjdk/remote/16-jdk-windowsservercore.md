## `openjdk:16-jdk-windowsservercore`

```console
$ docker pull openjdk@sha256:6124a032e025bc10f63a76f1044f5cb4323e6ccddd291e6b6eb9fd3bca87f4f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `openjdk:16-jdk-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:a4a62a3e4b818417d35ccfef83598c27b3723a4856d1cc33f69d62f612fb10ab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2867410352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f123dc13b8b03ba6057f8c16f66623bf51ff9ad071221d114284ec0101d5a070`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 00:31:04 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 00:46:34 GMT
ENV JAVA_HOME=C:\openjdk-16
# Thu, 14 Oct 2021 00:47:38 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 00:47:39 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 14 Oct 2021 00:47:40 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_windows-x64_bin.zip
# Thu, 14 Oct 2021 00:47:41 GMT
ENV JAVA_SHA256=9df98be05fe674066cc39144467c47b1503cfa3de059c09cc4ccc3da9c253b9a
# Thu, 14 Oct 2021 00:49:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 14 Oct 2021 00:49:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3778f0ab9c363534bcf1068a50329066ca025f6499401dd667a232ffdd9687e4`  
		Last Modified: Sat, 16 Oct 2021 00:35:18 GMT  
		Size: 349.3 KB (349328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5427b694905d6d6d09804a1db38a0b82f64f13b03e7455bc8b055b01219d09`  
		Last Modified: Sat, 16 Oct 2021 00:41:55 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae4ec65bd080afb62b76e06d690fae9131ea703a1ece1413d98c79097a99111`  
		Last Modified: Sat, 16 Oct 2021 00:41:55 GMT  
		Size: 310.7 KB (310663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bae148d5edb70207471fd19c8dd987430ccb73d0928764cbc7daae610232ad`  
		Last Modified: Sat, 16 Oct 2021 00:41:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcb8c911890f6f507a4fada1c3a915e757e0724d2e011c6264363c86cb5f704`  
		Last Modified: Sat, 16 Oct 2021 00:41:52 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01e9740f58d39e2bbca6832f33ced203e8fecfd22355aa2de72904c7999514b`  
		Last Modified: Sat, 16 Oct 2021 00:41:52 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351f79f369ecd8437e918d2d885caac68abda59f95ff2d15685e26bba496daf`  
		Last Modified: Sat, 16 Oct 2021 00:42:12 GMT  
		Size: 180.4 MB (180423062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb328aa229cd0e369173f960fd2e718e8a0691632daf133759f1d50f5a84d451`  
		Last Modified: Sat, 16 Oct 2021 00:41:53 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-jdk-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull openjdk@sha256:47960337f74b0de70987d46bb9db282fbacacfa8fc27b8b70d52fae91c3e096c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6453919271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b8355bf9dea30e49d36f0af06412e8164fe9f0b37a329365d115a3d42758953`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 12:40:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 00:35:32 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 00:49:32 GMT
ENV JAVA_HOME=C:\openjdk-16
# Thu, 14 Oct 2021 00:50:39 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 00:50:40 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 14 Oct 2021 00:50:41 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_windows-x64_bin.zip
# Thu, 14 Oct 2021 00:50:42 GMT
ENV JAVA_SHA256=9df98be05fe674066cc39144467c47b1503cfa3de059c09cc4ccc3da9c253b9a
# Thu, 14 Oct 2021 00:52:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 14 Oct 2021 00:52:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6974b1bd85ba3f9ce16d86231eced43f720fed9c13411d37584dfe7193bcde60`  
		Last Modified: Wed, 13 Oct 2021 13:27:57 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df06f60babff5e4f22bec0a3230e7cb06b975eee8a07f9541607a63c6f54ec1`  
		Last Modified: Sat, 16 Oct 2021 00:35:57 GMT  
		Size: 352.3 KB (352290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b62d10d8ed1fc98e10976304c9d6848ed7ee3a736a8b67975abc752ca21cda7`  
		Last Modified: Sat, 16 Oct 2021 00:42:34 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01244b88bb9a322597fc571785054bdf690c9c273715670823b5b0968550ca3`  
		Last Modified: Sat, 16 Oct 2021 00:42:35 GMT  
		Size: 348.9 KB (348900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787dfbc5c379796172eddf8fd38f5e651c5100a554c626e3ff6dd015ebea7032`  
		Last Modified: Sat, 16 Oct 2021 00:42:32 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02f5758e4c1e9f030367d25552048176620aa42c5935bf1ec008735eba1a43d`  
		Last Modified: Sat, 16 Oct 2021 00:42:32 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64da64eea29f440c4592f39b291504bf64028ddcda759a158828f49faf7fccd7`  
		Last Modified: Sat, 16 Oct 2021 00:42:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731380c26299e77fa281fb6a10504ee4755d349e13b9a45ebcb9ad677c55ae27`  
		Last Modified: Sat, 16 Oct 2021 00:42:50 GMT  
		Size: 180.4 MB (180443138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e3af3f531ea0158982fa55fb0bccb70af538c0e07960b294c8e2c3dc98dea2`  
		Last Modified: Sat, 16 Oct 2021 00:42:32 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
