## `eclipse-temurin:8u372-b07-jre-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:af7b97180f7b0b4028968dbbe2c7fd58533d59017d5ec2ce9c1bba5f86f3bc64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:8u372-b07-jre-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:80735aed6443d7313accd881cf69fec5b2d27afacd732c5357d38295faaae396
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1723063250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fbbb45fa429547642d04ecd9aaa0395f4d96f8e218ae91dea410c57b0de9643`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 00:40:08 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Sat, 24 Jun 2023 00:44:38 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_windows_hotspot_8u372b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_windows_hotspot_8u372b07.msi ;     Write-Host ('Verifying sha256 (34af6f80b9ad0351ce668a5e8968cfe9b83ee84776365320697aabe8a6d22e09) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '34af6f80b9ad0351ce668a5e8968cfe9b83ee84776365320697aabe8a6d22e09') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 24 Jun 2023 00:45:03 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:0cf20aa9a75b39e57d696d0bb3900b5cc5a492fd9ac8f4a17ff566f03670df6d`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166eeb481401c4148b669882cfd5f351623afc292a3bb3f6e6107c99fa275802`  
		Last Modified: Sat, 24 Jun 2023 01:25:41 GMT  
		Size: 72.1 MB (72056354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52c7cb6da82415125d1e3ae7a21b282c30e28c07aabd2b551d78a6ff36b2db9`  
		Last Modified: Sat, 24 Jun 2023 01:25:34 GMT  
		Size: 267.3 KB (267269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
