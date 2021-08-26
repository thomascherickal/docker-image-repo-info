## `eclipse-temurin:16-jdk-windowsservercore-ltsc2016`

```console
$ docker pull eclipse-temurin@sha256:70cab74cfeca9280149ad724dff87604e07e41953ed9281492609b162029c869
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `eclipse-temurin:16-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull eclipse-temurin@sha256:983155e77791dae3e063e2850585018ab63ba07a75df490093eb3db1dd161757
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 GB (6653713025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94eb54cb9447fb2db5308e0f0e849b8e5299b8db0ebf2825d29ce95879e1583a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 16:49:10 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Wed, 25 Aug 2021 16:50:48 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_windows_hotspot_16.0.2_7.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_windows_hotspot_16.0.2_7.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (b153c6ce102c6f05fd710c4b26c64224b649457613dad4830dcc6b551c0a4b3d) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b153c6ce102c6f05fd710c4b26c64224b649457613dad4830dcc6b551c0a4b3d') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-16' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 25 Aug 2021 16:51:55 GMT
RUN Write-Host 'Verifying install ...';     Write-Host '  javac --version'; javac --version;     Write-Host '  java --version'; java --version;         Write-Host 'Complete.'
# Wed, 25 Aug 2021 16:51:56 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34118a1198de824f2a68d546f879aa8137bdbd9ef7c68488df1124af810167f6`  
		Last Modified: Wed, 25 Aug 2021 23:33:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8ae51b0f710da62587ce5dde1106ce4c2cc1532ef20b0f88f1dae98ba3434e`  
		Last Modified: Wed, 25 Aug 2021 23:40:17 GMT  
		Size: 378.8 MB (378829746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836f6e5b3200e83c4a6763beb474375620bf97fb7e63d3292cc2f02c176a23e1`  
		Last Modified: Wed, 25 Aug 2021 23:33:45 GMT  
		Size: 3.9 MB (3912975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5642ca84b5ff92fbea692b90188f3e0b68d89019f23dc1b2ae79afc08a3aaee`  
		Last Modified: Wed, 25 Aug 2021 23:33:41 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
