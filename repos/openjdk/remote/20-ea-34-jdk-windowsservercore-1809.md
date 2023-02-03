## `openjdk:20-ea-34-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:574eac23ef76fdf7fbd22ea7e3bd6133b5aea09388324f2610c39f2f488fbe55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `openjdk:20-ea-34-jdk-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull openjdk@sha256:8008fd18f024680cfc80316f74c846db64174c4c943ecf3bcfa1f0f2c2969a6d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1902094600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ac84985e791dd0dc59509ef0ea653df122595b90af3d657ac2bdaca08b9bf0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:09:35 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 12 Jan 2023 05:13:49 GMT
ENV JAVA_HOME=C:\openjdk-20
# Thu, 12 Jan 2023 05:14:14 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 02 Feb 2023 23:28:47 GMT
ENV JAVA_VERSION=20-ea+34
# Thu, 02 Feb 2023 23:28:48 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/34/GPL/openjdk-20-ea+34_windows-x64_bin.zip
# Thu, 02 Feb 2023 23:28:49 GMT
ENV JAVA_SHA256=0387c564202f0ee1dc22d6316c79857a048210bf5d5de93fa23be9c88845b9a3
# Thu, 02 Feb 2023 23:30:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 02 Feb 2023 23:30:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fe1d317f0927d209417077d671ba0fb8e3b7ff9c583727da819f0d16252e80`  
		Last Modified: Thu, 12 Jan 2023 05:23:04 GMT  
		Size: 367.5 KB (367453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204fb4de92b3c2f3fbd44e35eab6a78c6001ee4da68e9f00b462472e9636c486`  
		Last Modified: Thu, 12 Jan 2023 05:25:04 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5262ccef5459e1e9f746ac49749d63fee0bb98296c21086879d1d379e8e7a`  
		Last Modified: Thu, 12 Jan 2023 05:25:04 GMT  
		Size: 320.0 KB (319987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2006a14e29afd20d2e82c5b305550ef19d62cb200531498ab84a5c8ec5ea908b`  
		Last Modified: Fri, 03 Feb 2023 00:26:24 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace58da48d2653f1a1f9a614b49ba91bf2a16ab5a1a42714843ac7d74b837491`  
		Last Modified: Fri, 03 Feb 2023 00:26:24 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb30b283c2c9a8188cf067a15cdf571610a49f76c2578aaa23cc7d2cb4864f3`  
		Last Modified: Fri, 03 Feb 2023 00:26:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e612d916d20b9dc406fcb26d8883858ced93065c35ea6ee4865b2eb2f5f5ece7`  
		Last Modified: Fri, 03 Feb 2023 00:26:46 GMT  
		Size: 193.5 MB (193454785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850d34e57a8bde1eb135566a4326e2ab395f3ededfaa0bc351ba49330711e4bc`  
		Last Modified: Fri, 03 Feb 2023 00:26:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
