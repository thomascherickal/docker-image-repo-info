## `adoptopenjdk:8-jre-hotspot-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:84afad9d22e077b5a96df4864fc23a4880efefeb5b12173e6d883bd7fc2a4e84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `adoptopenjdk:8-jre-hotspot-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull adoptopenjdk@sha256:8904899a56774988e2f493535a9216460ed77f2e80f114c2ef66b9f185a73639
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6345609023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:900bf13e9340df7fde78f610a9c3421c4552252f5704baa10d44e789ea2a2cfc`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 18:48:31 GMT
ENV JAVA_VERSION=jdk8u292-b10
# Wed, 11 Aug 2021 18:54:21 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_windows_hotspot_8u292b10.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_windows_hotspot_8u292b10.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (4365ea6d753ce61ce809fcd94e6cda1723673b3a79b4ca71a01599eb0aecef0a) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '4365ea6d753ce61ce809fcd94e6cda1723673b3a79b4ca71a01599eb0aecef0a') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:fe969d777c8422468f24927ce8709eeb00e997fd583536eacbc0b35e8f504de1`  
		Last Modified: Wed, 11 Aug 2021 19:58:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad5550774e84997e04c74a79ba2e3f446ca201687c48084cff6a978d86ccc0a`  
		Last Modified: Wed, 11 Aug 2021 19:59:50 GMT  
		Size: 74.6 MB (74640200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
