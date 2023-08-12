## `openjdk:21-jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:49ac5fea9b4b04874c83461896091808b29074a7cf08eae20e65c9e55d1a5ba2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1906; amd64

### `openjdk:21-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.1906; amd64

```console
$ docker pull openjdk@sha256:4ddb11bf530aa4bd0fbc85b94c7932bf326a9e6871644298099ec87807a04a02
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1996410036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78de6a19abbd21c0718df61098f9f35f77c5736d39241dcdef8c9404a777a8b1`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:36:45 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 10 Aug 2023 02:43:01 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 10 Aug 2023 02:43:22 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 12 Aug 2023 00:03:36 GMT
ENV JAVA_VERSION=21
# Sat, 12 Aug 2023 00:03:36 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_windows-x64_bin.zip
# Sat, 12 Aug 2023 00:03:37 GMT
ENV JAVA_SHA256=5434faaf029e66e7ce6e75770ca384de476750984a7d2881ef7686894c4b4944
# Sat, 12 Aug 2023 00:04:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 12 Aug 2023 00:04:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a18930eb7350c60f06351657db53550ff8c064f9f63673a2955eb64b696ffbd`  
		Last Modified: Thu, 10 Aug 2023 02:48:56 GMT  
		Size: 452.7 KB (452708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724681ec83ac29f19beeb1cb4fe664ac3de56a42d7f381314110fedb4f063463`  
		Last Modified: Thu, 10 Aug 2023 02:50:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ffe6018f3cff93f4bc90eacb1002f4cb347245b09e012b4071e3911805d7f0`  
		Last Modified: Thu, 10 Aug 2023 02:50:55 GMT  
		Size: 262.9 KB (262873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b382d1ceb03d95b96b76185b71a5a091d0a99eecd3a4fb6d6ed816617743d481`  
		Last Modified: Sat, 12 Aug 2023 00:10:35 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58819c441c3b6f1b063a9c67458eee1a1913a150101809677210542a129d0cc0`  
		Last Modified: Sat, 12 Aug 2023 00:10:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2943ab9a6cfa9c7e91442999ed5aa8f72200ff561e00f73c29fbe5ddf2c4072d`  
		Last Modified: Sat, 12 Aug 2023 00:10:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd04f7aa7695fc2e42fb9bcd6cd1c7d950786433853b833211d8123bfac7409`  
		Last Modified: Sat, 12 Aug 2023 00:10:55 GMT  
		Size: 198.3 MB (198322096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbf87844e75ad5696c70f1729a45e4b04bb1accbff36fbd9bac3b3c4d2114f3`  
		Last Modified: Sat, 12 Aug 2023 00:10:35 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
