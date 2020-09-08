## `openjdk:16-ea-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:61b906c59a7d0c373f2c34f491d8c6c66fc605b0878ee0ee678ddc11530ff228
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `openjdk:16-ea-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull openjdk@sha256:39299460a98028907da1ded3d95173ce0455673a1b16e88664b4be3aa5dcd70a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5956544945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a382868dc000aca8822952dd61bd6fd60423bea5da87ebeac73f8bbec93afd47`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Sep 2020 20:09:21 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Tue, 08 Sep 2020 20:09:22 GMT
ENV JAVA_HOME=C:\openjdk-16
# Tue, 08 Sep 2020 20:10:43 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 08 Sep 2020 20:10:44 GMT
ENV JAVA_VERSION=16-ea+14
# Tue, 08 Sep 2020 20:10:44 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/14/GPL/openjdk-16-ea+14_windows-x64_bin.zip
# Tue, 08 Sep 2020 20:10:45 GMT
ENV JAVA_SHA256=1b6ed89998fe831c6d9abb5d610675427775247f839acd698d367954ee8d4fdb
# Tue, 08 Sep 2020 20:13:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 08 Sep 2020 20:13:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbeff382f1371b6819ca1ae810348afda32084cbd4526c4114c9ff5f85a5d6d`  
		Last Modified: Tue, 08 Sep 2020 22:28:21 GMT  
		Size: 9.9 MB (9886373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ce5a5f1c846bc13c012040ba007559f48bfa1c47939f5ef2dd12a157bf9e45`  
		Last Modified: Tue, 08 Sep 2020 22:28:16 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7769f3897b358df537321f97bab12aff9a86e616ddaa588c3b91db0d0b65c1`  
		Last Modified: Tue, 08 Sep 2020 22:28:17 GMT  
		Size: 5.3 MB (5336442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44503f4a45f1d6b463b61a8471b323e93ca7e09452f87e2070c8114d68b713c5`  
		Last Modified: Tue, 08 Sep 2020 22:28:13 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcd635d0dd2966b8cd7b3ecdb0b6064cbc17ebb69ce36d6f778de42c90dd57a`  
		Last Modified: Tue, 08 Sep 2020 22:28:13 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679242c149aacbb3c0922802b29a8248b53a53e6402b0740c98b51c99f0a252e`  
		Last Modified: Tue, 08 Sep 2020 22:28:12 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1d009d40c39e81f1ae715f014151dd5067e6e6e7126a405b1dc78d6df255fe`  
		Last Modified: Tue, 08 Sep 2020 22:28:35 GMT  
		Size: 202.1 MB (202060841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707f18a9be56bc6ef5a9af7ea41c3a05628bf8b209605a09ddf761c26ec5e4d1`  
		Last Modified: Tue, 08 Sep 2020 22:28:13 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
