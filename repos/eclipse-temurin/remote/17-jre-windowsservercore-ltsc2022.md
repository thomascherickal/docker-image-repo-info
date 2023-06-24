## `eclipse-temurin:17-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:fb525e333c3fb0021d366d1e057eeefbbf5e53f2e1f16688808476075203359d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:17-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:196a3035ffd952265666a311e505352bd3f2566c8291d481b916fc4770e41b8d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1501053449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a15325bc65ffdad277399636ecf4c45a2826fe0a355b97870755bf01083ac3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 00:52:35 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Sat, 24 Jun 2023 00:57:34 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_windows_hotspot_17.0.7_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_windows_hotspot_17.0.7_7.msi ;     Write-Host ('Verifying sha256 (fa3f8202b9d748c320604c08a9748163372c3ea4aeeb64c43d4b6a3b56842ff4) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'fa3f8202b9d748c320604c08a9748163372c3ea4aeeb64c43d4b6a3b56842ff4') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 24 Jun 2023 00:58:31 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e50a244c62c5b773beebfcdac06077745d5ae460eae34334bb1740c369f3eb`  
		Last Modified: Sat, 24 Jun 2023 01:28:49 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289455d4b3a1a7cd6eb45955e58ee5c52f2dc508a13b13e86a6a52b678e863d5`  
		Last Modified: Sat, 24 Jun 2023 01:30:48 GMT  
		Size: 74.5 MB (74482155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d251ece40a6f1eef4a44e0712c78d92a5b2f7ccebcb046c4a890c3d30be3f6c`  
		Last Modified: Sat, 24 Jun 2023 01:30:38 GMT  
		Size: 269.9 KB (269862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
