## `openjdk:jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:c396d571e3c6c13feac83ecc251ac81d774b9ac9042f52f8966dc72d73d8922f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `openjdk:jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull openjdk@sha256:74933bcf109f5430b38a147738f514f92f5584bbf4d88f4916479d0f5c024bf1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6452017389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78810f775a0240d86a2f00d6bc06d0a60b802f52239be3d20278379a142f3ea6`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 17:26:21 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 11 Aug 2021 17:44:00 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 11 Aug 2021 17:45:33 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 11 Aug 2021 17:45:36 GMT
ENV JAVA_VERSION=16.0.2
# Wed, 11 Aug 2021 17:45:39 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_windows-x64_bin.zip
# Wed, 11 Aug 2021 17:45:41 GMT
ENV JAVA_SHA256=9df98be05fe674066cc39144467c47b1503cfa3de059c09cc4ccc3da9c253b9a
# Wed, 11 Aug 2021 17:47:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 17:47:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85818d8ae526f813cf82bc85044b12bcf64737f7bce6c6b2d983a6db1251a488`  
		Last Modified: Wed, 11 Aug 2021 18:20:44 GMT  
		Size: 348.4 KB (348421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59205a8ba2ea45f517ddce94ffb12851b0152552900fa75375c7c04fa99f225`  
		Last Modified: Wed, 11 Aug 2021 18:27:33 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccec5537463da715765022be943cfcfbb7884e045b1c704edee65d25ea4e631`  
		Last Modified: Wed, 11 Aug 2021 18:27:33 GMT  
		Size: 301.7 KB (301653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368b26c690f6dd79551dbf6e3d0ae7fbe5df3182d0f2d5d0fc61a1706bf416c6`  
		Last Modified: Wed, 11 Aug 2021 18:27:30 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f92e0052c05d2d24203b1816364beb8839d349a31182bb660af608c1ebd070d`  
		Last Modified: Wed, 11 Aug 2021 18:27:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c148b54fa297a818a235cbe2f9d46af256efcc771d98a08780e14d42dd51af28`  
		Last Modified: Wed, 11 Aug 2021 18:27:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c25a95ff37c438cd932d2bbeea875a86d4f2e69117962749c60117cb5d5d59`  
		Last Modified: Wed, 11 Aug 2021 18:27:51 GMT  
		Size: 180.4 MB (180392748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5b39f4043311c4a190a1a1f8f072ecf170dab94c5a912dffa43d389afe3b74`  
		Last Modified: Wed, 11 Aug 2021 18:27:30 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
