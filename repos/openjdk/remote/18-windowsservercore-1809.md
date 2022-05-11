## `openjdk:18-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:580991a5b34f0b96ac9af6b8d3312902b9bd4dfddd13344e7ccdbca6cef91e93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `openjdk:18-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull openjdk@sha256:4a72353f3c97c13ba4ae7aae7cde32396c7bb441519e7db0c13a034ff9260f45
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2689418336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a2f4a9498163fca3a2220f56f523d3773e9241017158679de22e602372cf45c`
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
# Wed, 11 May 2022 15:35:58 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 11 May 2022 15:36:47 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 11 May 2022 15:36:48 GMT
ENV JAVA_VERSION=18.0.1.1
# Wed, 11 May 2022 15:36:49 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk18.0.1.1/65ae32619e2f40f3a9af3af1851d6e19/2/GPL/openjdk-18.0.1.1_windows-x64_bin.zip
# Wed, 11 May 2022 15:36:50 GMT
ENV JAVA_SHA256=a970b922a05a7fc2b077c89bf96c74570f65695b2ba067dc81805107517d7fed
# Wed, 11 May 2022 15:38:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 11 May 2022 15:38:05 GMT
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
	-	`sha256:29f77a3db231e908db7142966bed2dd4e23572838d9971e6e6bbc15f6766810f`  
		Last Modified: Wed, 11 May 2022 16:08:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ea510b06a7fadc94852cc46f8c6f7958bddb30317d7199c382ed48767ac4e`  
		Last Modified: Wed, 11 May 2022 16:08:09 GMT  
		Size: 317.4 KB (317415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a684287a8e478b049d7812398362103aa34475645143ca779bdced85322c4eb8`  
		Last Modified: Wed, 11 May 2022 16:08:06 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0727c45e1567e9c59e036e254bb9311cbf0c59a96605cb977ceae700dade80`  
		Last Modified: Wed, 11 May 2022 16:08:06 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba93c0281b48e74f1342bc74ceb0af95f737b92a2c93b425338d5dc31e5c1c8`  
		Last Modified: Wed, 11 May 2022 16:08:07 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3f40aaa2da5550c00c083e66b2a924ef164b5134083e693d81ccaeafa28c40`  
		Last Modified: Wed, 11 May 2022 16:11:12 GMT  
		Size: 184.5 MB (184548826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f3a1929091ca223d6419cdcbdb9591b1f96ab10d3199f4c8bf390f2d2d3884`  
		Last Modified: Wed, 11 May 2022 16:08:06 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
