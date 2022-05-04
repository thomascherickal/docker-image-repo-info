## `eclipse-temurin:18-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:015fc5b340aa95a7645edd20069c14639bc8edb333e95a8f15c50eb7e2fdbdf6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `eclipse-temurin:18-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:7a8045e81d202befd1263a0cce041aa6882c8360c1171861c7a5a1551b75307d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2301859793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dcb5bbbd41e40b01cd73b45300759abf34d885bb9c135832c591991fe2df60b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 04 May 2022 18:17:37 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 04 May 2022 18:24:30 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_windows_hotspot_18.0.1_10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_windows_hotspot_18.0.1_10.msi ;     Write-Host ('Verifying sha256 (75a0749dfdec3f7238b0ba2572ff9b2f7debbb56710531b960d60769b1b070f5) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '75a0749dfdec3f7238b0ba2572ff9b2f7debbb56710531b960d60769b1b070f5') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-18' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 04 May 2022 18:24:53 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39da655b2390ca6c77bb41f8a18aba94d81f7ed3ca9716c950549ed4ddae8201`  
		Last Modified: Wed, 04 May 2022 18:32:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8c7bc7a61cfef254e0ed36ea32f733fc1405e25efa0da974d243407a02ba44`  
		Last Modified: Wed, 04 May 2022 18:35:16 GMT  
		Size: 74.3 MB (74325454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2003e01275aa784ee35da8228f96d7a92ecbe4c96df4176b3e895d9c6b3cc37b`  
		Last Modified: Wed, 04 May 2022 18:34:00 GMT  
		Size: 576.7 KB (576658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
