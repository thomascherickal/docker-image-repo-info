## `eclipse-temurin:8-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:9cb2d8567fe3433645a3abfd07bb27733dd77d3a2d6cd7ec3ff58974fefca3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `eclipse-temurin:8-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:f8ad347ffd12c1350810c2c8bd94ede3f6021d0ce0a463104b6ea1f857068581
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2298441907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd0056aba17a339d4e78f63904e18b82039333e270180cd7755c693199bc128`
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
# Wed, 13 Apr 2022 15:17:22 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_windows_hotspot_8u322b06.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_windows_hotspot_8u322b06.msi ;     Write-Host ('Verifying sha256 (74eb66d2d6aefdc42f95681616c94f6a41b1e133d899131719cf8c2f0cbf0a25) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '74eb66d2d6aefdc42f95681616c94f6a41b1e133d899131719cf8c2f0cbf0a25') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Apr 2022 15:17:42 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:fab434ffd135ddf5af18fe93e1ad179804267075ef210d9abb3a5d5e82be3729`  
		Last Modified: Wed, 13 Apr 2022 16:01:45 GMT  
		Size: 70.9 MB (70907466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d6b46a5fa5bbc83919aa67f1dd953eff5ba5eeb337cd8e2132b8e4a073b700`  
		Last Modified: Wed, 13 Apr 2022 16:00:28 GMT  
		Size: 576.9 KB (576852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
