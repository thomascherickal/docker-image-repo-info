## `eclipse-temurin:8-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:c000e122ddcf22199bebc2731e8021ee5a16d2e0dbad4fba4c1535e483b4017f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `eclipse-temurin:8-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull eclipse-temurin@sha256:0fa322220f5173416ec1336e6939cf1b876839b5295eb5332d68bfb5f5252b99
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1847409294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c1d6906d8c5c52153849559cfe57fb68feff33394946c1cd8cbcc7a5db6cc6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 00:35:06 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 10 May 2023 00:41:30 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_windows_hotspot_8u372b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_windows_hotspot_8u372b07.msi ;     Write-Host ('Verifying sha256 (34af6f80b9ad0351ce668a5e8968cfe9b83ee84776365320697aabe8a6d22e09) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '34af6f80b9ad0351ce668a5e8968cfe9b83ee84776365320697aabe8a6d22e09') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 May 2023 00:41:54 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d811256e9932f5246aaec94ff3b6652abba4c9852dda789b9f0bfca1dabdee22`  
		Last Modified: Wed, 10 May 2023 06:54:26 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920c2420f8f51bd158f07db91af726a7effc4564f99f5f5c8db7cb1726592189`  
		Last Modified: Wed, 10 May 2023 06:55:47 GMT  
		Size: 72.2 MB (72159725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de40b51c940c113cc94bf38aa5f871b1809a264a5758447a70b1bdb660ee2aa9`  
		Last Modified: Wed, 10 May 2023 06:55:40 GMT  
		Size: 265.2 KB (265247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
