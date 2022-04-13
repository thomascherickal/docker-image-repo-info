## `eclipse-temurin:8u322-b06-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:bfe65cce1f656d184542227e270b83600f932b30bd584fd534e9100869e1bb92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `eclipse-temurin:8u322-b06-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:419bf6637fa48141bec8d42c5d4113bd39db906816e779abed0b81bb2b82b079
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2417168716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf400da2c8f89545a697732e815add96118204a7067e534269624cc5afb7f14`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 15:12:15 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Wed, 13 Apr 2022 15:13:01 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_windows_hotspot_8u322b06.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_windows_hotspot_8u322b06.msi ;     Write-Host ('Verifying sha256 (e9337d5bba9b60a9d00a939fecb05718b2303023a587da6ae4862080714f9f0b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e9337d5bba9b60a9d00a939fecb05718b2303023a587da6ae4862080714f9f0b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Apr 2022 15:13:37 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:c8f928df4aebcabe565eb4cb6d5dbbf1ac28479dac45dbdfc3b86d72daaed813`  
		Last Modified: Wed, 13 Apr 2022 15:54:03 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1716ed12c5f82c6669680df9dd478a49edf9427b317086a7d3d7e6b1ab688c42`  
		Last Modified: Wed, 13 Apr 2022 15:57:22 GMT  
		Size: 189.6 MB (189635690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f06d80bb91e7820986833a257d7d394eb252930eddc722a55d9a41ba790b37`  
		Last Modified: Wed, 13 Apr 2022 15:54:03 GMT  
		Size: 575.4 KB (575437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
