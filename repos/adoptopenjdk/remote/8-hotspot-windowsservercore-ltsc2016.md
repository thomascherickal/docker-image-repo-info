## `adoptopenjdk:8-hotspot-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:1d1f5058e22824c193b5d82b7e5bff7a92a65f8b0804161bb726e60e111b7671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `adoptopenjdk:8-hotspot-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull adoptopenjdk@sha256:ec7c35d1a1015a4fa400ed7ba140cbcafa744d9b7e8125a38f6d3e7a683284c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5994267113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:815b8d8cd16ae14a42fd6c0a59a3959299aa8c5eda3e83abf6f2466471815ef1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 17:39:02 GMT
ENV JAVA_VERSION=jdk8u292-b10
# Wed, 12 May 2021 17:41:08 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_windows_hotspot_8u292b10.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_windows_hotspot_8u292b10.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (f6bd2e351a451b8dc7ed19d44b18a27ff8a0602016625fac5134c4defe5e560c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f6bd2e351a451b8dc7ed19d44b18a27ff8a0602016625fac5134c4defe5e560c') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3ca54eb315d19066b7a65006d54d7439cf5c6bd365d360b56888ece9635944`  
		Last Modified: Wed, 12 May 2021 18:55:08 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096408f2ebf687ec5808d5083de6a4b724688a2d203600a1256f9160d84fe3f6`  
		Last Modified: Wed, 12 May 2021 18:55:32 GMT  
		Size: 198.5 MB (198486998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
