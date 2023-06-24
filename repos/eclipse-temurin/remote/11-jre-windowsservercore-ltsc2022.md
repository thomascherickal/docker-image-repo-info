## `eclipse-temurin:11-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:1a9b7a67477e5917a263d9b86509425fc9d1c25ae4bad5f8dc668a8bbebbc8fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:11-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:bb654525ac236486cd1fb3fcfd9255881160cf44f25d0d2784d51f43d9e26bbf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1500851418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:350e4e6dd779f09b51a241f6737c3c6797f5d7fbcff923b687553a2f4c6e29ca`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 00:45:32 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Sat, 24 Jun 2023 00:50:28 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_windows_hotspot_11.0.19_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_windows_hotspot_11.0.19_7.msi ;     Write-Host ('Verifying sha256 (4556ea75ccc16f762f661675bd8a22e64b52890fa2fb330729316e120791ac09) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '4556ea75ccc16f762f661675bd8a22e64b52890fa2fb330729316e120791ac09') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 24 Jun 2023 00:50:50 GMT
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
	-	`sha256:45d4e28c1d2928452bdeb42928074a54917a77f5983ee5acd013a6969bd5d694`  
		Last Modified: Sat, 24 Jun 2023 01:26:05 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912837fdbc0bbdbc9cea2e8ab68895c565c4eedf75e166b4f23c00d589523a74`  
		Last Modified: Sat, 24 Jun 2023 01:28:04 GMT  
		Size: 74.3 MB (74273165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a0d2156d8024a10ce47c785c808633518c9be9e9c835a5c0dc908584d24da2`  
		Last Modified: Sat, 24 Jun 2023 01:27:54 GMT  
		Size: 276.9 KB (276899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
