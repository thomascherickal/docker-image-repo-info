## `openjdk:20-ea-windowsservercore`

```console
$ docker pull openjdk@sha256:8ed2b388025bcc5af0b1816a97cd6f3ec0dbb72743bdbb864207294d7a514e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1129; amd64
	-	windows version 10.0.17763.3532; amd64

### `openjdk:20-ea-windowsservercore` - windows version 10.0.20348.1129; amd64

```console
$ docker pull openjdk@sha256:7a6a20d528401b6e71384ea271753db9a7716a841496cb80024f86a1afcd3bd0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2609823249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77976566eb67139b02673c55284f4a152b6d0931e428dfdf6d7a7bd1af7a6052`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:39:02 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:39:03 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 12 Oct 2022 16:39:22 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:39:23 GMT
ENV JAVA_VERSION=20-ea+18
# Wed, 12 Oct 2022 16:39:23 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/18/GPL/openjdk-20-ea+18_windows-x64_bin.zip
# Wed, 12 Oct 2022 16:39:24 GMT
ENV JAVA_SHA256=2957954de0bb9cde44f6893f02d9a175cdcbb470cd3650080bf53f05472fe6b5
# Wed, 12 Oct 2022 16:40:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:40:10 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cbc434576dbff410ee0aa4228c6f0fa038ee64fba58d8b81df98ab5bd3e8e5`  
		Last Modified: Wed, 12 Oct 2022 16:51:49 GMT  
		Size: 609.6 KB (609572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d05c1a9fc44de33350221b30e908eaeae6d05eba0fe481490fe562a59dc8fc`  
		Last Modified: Wed, 12 Oct 2022 16:51:49 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71e1244e1a09ac39ec09321d2cf652a948c02d0366d860e30695700811edad3`  
		Last Modified: Wed, 12 Oct 2022 16:51:49 GMT  
		Size: 524.9 KB (524924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b89d2beb154f70c0bb839e18c5aea972af8547b86e7943656825689c663f868`  
		Last Modified: Wed, 12 Oct 2022 16:51:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca0133330c55b43a5b9b2a98b18ceeb150c96f62e57609a5ade907a6d1e3188`  
		Last Modified: Wed, 12 Oct 2022 16:51:46 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c2e59cd26188baba5e5869df51161da90c7e38b65042afcb52bf2e8c6e5cff`  
		Last Modified: Wed, 12 Oct 2022 16:51:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725284b7bb06aabe785a90cf3e99785e21a9bbf53a23f038c1bc23ec26c66cad`  
		Last Modified: Wed, 12 Oct 2022 16:52:05 GMT  
		Size: 192.5 MB (192456966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285ed69fccf0f1c837f1a3d74adc57233741bafa41dab4f45dfba63c9d196622`  
		Last Modified: Wed, 12 Oct 2022 16:51:46 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull openjdk@sha256:dc670be6af607ac02a191d185c64cc1008d20a7d836aa466736bc0a20e558efe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2904078808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651929bc6bfe7d328432a46eac7fb0babafedd981eeb76b042bccd3217302791`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:41:21 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:41:22 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 12 Oct 2022 16:42:14 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:42:15 GMT
ENV JAVA_VERSION=20-ea+18
# Wed, 12 Oct 2022 16:42:16 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/18/GPL/openjdk-20-ea+18_windows-x64_bin.zip
# Wed, 12 Oct 2022 16:42:17 GMT
ENV JAVA_SHA256=2957954de0bb9cde44f6893f02d9a175cdcbb470cd3650080bf53f05472fe6b5
# Wed, 12 Oct 2022 16:43:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:43:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891dd6ec2fa598da717e21a05ad77857caf95e46fc5861ed7e79aab507e9fd11`  
		Last Modified: Wed, 12 Oct 2022 16:52:29 GMT  
		Size: 347.9 KB (347943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e673f50a0247a96d4f10904fad919663c061d29e5445b3531a1eb3a227b99657`  
		Last Modified: Wed, 12 Oct 2022 16:52:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f4cce28740d1d55be90dac59ca06df221cfd3100dd82e1eedd5a929a54b2cf`  
		Last Modified: Wed, 12 Oct 2022 16:52:29 GMT  
		Size: 310.8 KB (310762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53499526da774696bf07848d0cf1228f65553efa7c1d44b56fa922b8ba04a8d6`  
		Last Modified: Wed, 12 Oct 2022 16:52:26 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259c257b7c27f83c2258883fddd044336866ad82c60d334348f46e9b866913b9`  
		Last Modified: Wed, 12 Oct 2022 16:52:26 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cc9648e405a0ade4b2a268c2ec34e8dc624143d49792539a4ea460598fe748`  
		Last Modified: Wed, 12 Oct 2022 16:52:26 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99f33c1c7d8b3e24b29fa13139837ae0f5820bd3929fecaca979ed1d616715c`  
		Last Modified: Wed, 12 Oct 2022 16:52:45 GMT  
		Size: 192.2 MB (192247675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4497071f446e01882bca90ace1a5e83e8c8b5740facc27c71c8cf42ec15e2b6`  
		Last Modified: Wed, 12 Oct 2022 16:52:26 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
