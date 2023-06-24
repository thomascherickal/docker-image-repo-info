## `eclipse-temurin:17-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:e5e66c1175326171b1f1e3b3838f3a9a81c10c28c3a845a20d7c74ed2358142b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:17-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:f5afab924cb33696c99b9b033f4772ea5ce461455bc538658b1927d180ad5a96
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2007243340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:373b75f8cd415f62a2ea7b85b979af06ac76c1dadc35f190ee089a1a159aaacf`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 00:54:20 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Sat, 24 Jun 2023 00:55:20 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_windows_hotspot_17.0.7_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_windows_hotspot_17.0.7_7.msi ;     Write-Host ('Verifying sha256 (a295dff1fd9af8341f9483202a0a96fab191438c1417c32d1f5d9ceff5927a1b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'a295dff1fd9af8341f9483202a0a96fab191438c1417c32d1f5d9ceff5927a1b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 24 Jun 2023 00:55:46 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Sat, 24 Jun 2023 00:55:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f356396592fe230f5584c07513ea267622004ca2c3e06f8fbab54a86e0e96f2`  
		Last Modified: Sat, 24 Jun 2023 01:29:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357c75f4124058de7dbd827f829533b1d37bc21c47881ae52ca0a4d3b7961f2`  
		Last Modified: Sat, 24 Jun 2023 01:29:55 GMT  
		Size: 352.7 MB (352667486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db879bdd8b3b2470d2373a51a439332586f7b00056f86cbbfd223d7c42af6d6`  
		Last Modified: Sat, 24 Jun 2023 01:29:29 GMT  
		Size: 3.8 MB (3834961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3913f56d0e52692e7c4482fca2cd1407d02e11a1ed6eb1d8dd1f8a2f474051b1`  
		Last Modified: Sat, 24 Jun 2023 01:29:27 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
