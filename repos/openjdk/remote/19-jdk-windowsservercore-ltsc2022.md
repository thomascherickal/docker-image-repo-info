## `openjdk:19-jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:95ad3cc1758d842f00eb3e428494109e106cd573b7324a2c7c27feee10110cab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `openjdk:19-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull openjdk@sha256:071ab8a578f716bb9c985052536b0916aeb1ab3679fb8943decbaf6f68792e2d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2509841803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3cb1277fe0cbd14d2392e2a1d0dc94e2940ce864e31f7729d05742468a5a8e3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 16:55:00 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 10 Aug 2022 17:01:00 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 10 Aug 2022 17:01:20 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 10 Aug 2022 17:01:21 GMT
ENV JAVA_VERSION=19-ea+34
# Wed, 10 Aug 2022 17:01:22 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_windows-x64_bin.zip
# Wed, 10 Aug 2022 17:01:23 GMT
ENV JAVA_SHA256=5d3ac1a89d92a142588bc8546aa737c37d1971bcff17810b5ff947790c97e623
# Wed, 10 Aug 2022 17:02:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 17:02:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0cc935c154780815cf1fb6065aa1c262b52a7648b984b06133beb4e95833c0`  
		Last Modified: Wed, 10 Aug 2022 17:27:08 GMT  
		Size: 624.7 KB (624700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c321b8aceb5aa354374c98f1ed5eb3ebe9da9235dfb65eaecf437c95f17a9372`  
		Last Modified: Wed, 10 Aug 2022 17:29:18 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06331a3f3c54ed0599c9730f358b1a0548e4df17ed5dc21bacce5929cb4424e5`  
		Last Modified: Wed, 10 Aug 2022 17:29:19 GMT  
		Size: 557.1 KB (557139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6df01a94acd9dc2ffe2ca5fb6a1e7d8da2339fb2dfac3badd2562a04895303`  
		Last Modified: Wed, 10 Aug 2022 17:29:16 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a107949c17d548c8498bd505865892aead1d7a4ee2dde70f9280619b10c12d6`  
		Last Modified: Wed, 10 Aug 2022 17:29:17 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8852ccb6abf7049ca6174c9ae98a324bce09838dcdc08940c2388cef3cb6af8d`  
		Last Modified: Wed, 10 Aug 2022 17:29:16 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee34c08298e6f8f7ea4e4137fff85e2ddf8c24fe9c3d817bee65fd639ff4a1a1`  
		Last Modified: Wed, 10 Aug 2022 17:29:38 GMT  
		Size: 191.8 MB (191762282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c483e898d8717d7eaf30a218bbd8d5a170a89eb170c44265f14bcefea74d75f4`  
		Last Modified: Wed, 10 Aug 2022 17:29:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
