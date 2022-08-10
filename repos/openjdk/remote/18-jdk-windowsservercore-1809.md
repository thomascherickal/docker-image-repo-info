## `openjdk:18-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:b8a815d10a60f2dc78119b8a0b126c7133fcb853fd87e329c5706fb97a5bc531
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `openjdk:18-jdk-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull openjdk@sha256:73436d7c18d665cb4322aa8239aaef24f89bd59fe0959fdc79ce93e9d507620a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2862923150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa88c4e78b37108fc0e62fb632bc5f6f4bcb345b9765995bd301feaae8f8d47d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 16:57:20 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 10 Aug 2022 17:07:09 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 10 Aug 2022 17:08:05 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 10 Aug 2022 17:08:06 GMT
ENV JAVA_VERSION=18.0.2
# Wed, 10 Aug 2022 17:08:07 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk18.0.2/f6ad4b4450fd4d298113270ec84f30ee/9/GPL/openjdk-18.0.2_windows-x64_bin.zip
# Wed, 10 Aug 2022 17:08:08 GMT
ENV JAVA_SHA256=441f2bfa18f318995d305d06c2326b1145b27dd08521cef5dacc561867cfee5c
# Wed, 10 Aug 2022 17:09:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 17:09:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9df80b59d75310c5b623001e9a6fefa8c2f0255dfbb8c58e60daa3aba0f9c6`  
		Last Modified: Wed, 10 Aug 2022 17:27:52 GMT  
		Size: 347.3 KB (347323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97034bfcb94cc788a4eaf71df59ed07028db63329f1f21ddb15633b5c675add`  
		Last Modified: Wed, 10 Aug 2022 17:32:12 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6243a4ee8745358b40745425fc03c45d45c41029a93b1100d133f94d8f95162`  
		Last Modified: Wed, 10 Aug 2022 17:32:13 GMT  
		Size: 309.9 KB (309896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a6906238139be99eaf1af5c772a7f575137f747221c23f93b0ed54a460cc6e`  
		Last Modified: Wed, 10 Aug 2022 17:32:10 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ebce489c8d25f0b333621b98a27086b2d96483a6addffeeddbd85d84cf1f1f`  
		Last Modified: Wed, 10 Aug 2022 17:32:10 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc09ba54353a29024ca70400344ff2ade2b7a26067a6f89369c3181099b9a80`  
		Last Modified: Wed, 10 Aug 2022 17:32:10 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d9c94841bff112eca52961f6656de57572159e6da77c0041de7c7cbedc5766`  
		Last Modified: Wed, 10 Aug 2022 17:32:30 GMT  
		Size: 184.5 MB (184544660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b68535bf7d23c3eda9d173065eb6ad77a75cec91e744f31ee69b75b3e9a575`  
		Last Modified: Wed, 10 Aug 2022 17:32:10 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
