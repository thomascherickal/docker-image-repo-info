## `openjdk:19-ea-21-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:c2ddeb2854414ef65e13adff053d1f128a103bdec14e1336a2fdbd1be07220bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `openjdk:19-ea-21-jdk-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull openjdk@sha256:59f7b731cb930aed39fdd239cc9b6501a6d9261925f8e282ace8c5f12d71c8f5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2695016313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06f4333ac1075dd360418b4235b771a52f374ef04ecb39180958d1eb964ae386`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 15:31:20 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 11 May 2022 15:31:21 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 11 May 2022 15:32:04 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 11 May 2022 15:32:05 GMT
ENV JAVA_VERSION=19-ea+21
# Wed, 11 May 2022 15:32:06 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_windows-x64_bin.zip
# Wed, 11 May 2022 15:32:07 GMT
ENV JAVA_SHA256=8445436e394bb7413fb586515b5681989aafbcbf448616a1f850550b9d07da47
# Wed, 11 May 2022 15:33:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 11 May 2022 15:33:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d16e9483c31353bee635610112700e2b9f38d45e154c79f5331ff07164b3f07`  
		Last Modified: Wed, 11 May 2022 15:56:46 GMT  
		Size: 488.1 KB (488114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3edb7b7391c69a83de5498a0df582da9d86d3dd21d40664b920bc4c45a896b`  
		Last Modified: Wed, 11 May 2022 15:56:45 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009f37a60cc36209d3b0aac27db2934d6ddfb285c5845c2dd7227945d3aff595`  
		Last Modified: Wed, 11 May 2022 15:56:46 GMT  
		Size: 317.1 KB (317078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fec896afd06ddcc8ac974a41c9d4534d24768001c1b407ff2a07c3ae3c87b4`  
		Last Modified: Wed, 11 May 2022 15:56:43 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b624fe18ad4420cee10388986d7c4cab34212cd771cea325fe55924a77483d6b`  
		Last Modified: Wed, 11 May 2022 15:56:43 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97271dc418efc5f8b20bd1e2e5e283596c17b1aea946fae956fe6bc5c0ce6baa`  
		Last Modified: Wed, 11 May 2022 15:56:43 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d076092a392c1f6caab3e5e8a0b2558186d120bf54fda19bc3a350a75beacc`  
		Last Modified: Wed, 11 May 2022 16:00:03 GMT  
		Size: 190.1 MB (190146804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc23dd47cf69d7446c08a0ba59eeb08827731b05d939a24a61fddbada2e6669c`  
		Last Modified: Wed, 11 May 2022 15:56:43 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
