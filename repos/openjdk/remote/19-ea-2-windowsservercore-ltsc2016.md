## `openjdk:19-ea-2-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:796458c910f67f41e8f900514f0b056d93b2ab11afff4cad9ff8b3696cd59d8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `openjdk:19-ea-2-windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull openjdk@sha256:9ee471d7a74fd2136a67162c79e5c92b4fc805d055317ab7f27f2d59a0c074ec
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6460501696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d043157bfb42bddd25c9ac53f3e6d6066e4754122e3d1604b58b23bd2c8aaa`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 06:59:56 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Sat, 18 Dec 2021 06:59:58 GMT
ENV JAVA_HOME=C:\openjdk-19
# Sat, 18 Dec 2021 07:01:04 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 18 Dec 2021 07:01:04 GMT
ENV JAVA_VERSION=19-ea+2
# Sat, 18 Dec 2021 07:01:05 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/2/GPL/openjdk-19-ea+2_windows-x64_bin.zip
# Sat, 18 Dec 2021 07:01:06 GMT
ENV JAVA_SHA256=d26510cea1e738a5363deb9923765036d1a3e64c993e5f0b3c922b8986e1dac6
# Sat, 18 Dec 2021 07:02:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 07:02:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f88306d11f630889687486bb566861161592f87bc40ac9850fce316e5b7780`  
		Last Modified: Sat, 18 Dec 2021 10:55:53 GMT  
		Size: 335.8 KB (335827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156b98596a6a205c44cb60ec59ad014ee89440f058f3461f521ffc899670dc95`  
		Last Modified: Sat, 18 Dec 2021 10:55:53 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52478147df3d18fbcb95a25b68742ff25cdb15025a1d754d61d54486c9151339`  
		Last Modified: Sat, 18 Dec 2021 10:55:53 GMT  
		Size: 329.4 KB (329409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba7bc0230a84508b2058864fa7267863d67cfa599a0e487c837d957139a950c`  
		Last Modified: Sat, 18 Dec 2021 10:55:50 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14da3ca85c674d4751e0cb022027aa2283057feb3becc869308bb5b4101b9c8`  
		Last Modified: Sat, 18 Dec 2021 10:55:50 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92743355506213cf70c7eb7fa6aa0720bd0e8e0aae2e43933209005a789dce9`  
		Last Modified: Sat, 18 Dec 2021 10:55:50 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948f85483cabce9b56e8aa34a7af386da3fd2ae93b76788a5b9e7c841db24eb6`  
		Last Modified: Sat, 18 Dec 2021 10:56:11 GMT  
		Size: 185.1 MB (185113281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e1ee1b2fe43691c50b46bcf55e85083ffa74ae1f488884fe1b71bca3f2686e`  
		Last Modified: Sat, 18 Dec 2021 10:55:50 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
