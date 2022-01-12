## `eclipse-temurin:8u312-b07-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:82511380ca3c703cfaee168a6ddd6811b9fead71041f667941d4502f4021dbe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `eclipse-temurin:8u312-b07-jdk-windowsservercore-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull eclipse-temurin@sha256:deee37442415d9209dab9c6c033058b79ee09f15071c89f45ce4a034c62c9106
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2901864553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac019f1e92cd16b981c61d9a97a7daa7caf8c6ef70ccd912f96be087c144bb14`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 05:11:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 15:31:05 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 12 Jan 2022 15:32:46 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_windows_hotspot_8u312b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_windows_hotspot_8u312b07.msi ;     Write-Host ('Verifying sha256 (5544ebcb03206f3c3f5f19f6da03003a154cb2b489a06d88a052792f72b76c21) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '5544ebcb03206f3c3f5f19f6da03003a154cb2b489a06d88a052792f72b76c21') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 12 Jan 2022 15:33:55 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3a70d5fd54e2005efbf590b48700ed40509210354a0d8f3f18c3b444a5325896`  
		Last Modified: Wed, 12 Jan 2022 06:20:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1440152d7fe8d63c5c9773cf2bbc39cd20d7d90bc195ba351f6795634011b`  
		Last Modified: Wed, 12 Jan 2022 16:01:37 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa99d61a2837c3c05a5aec7666c1fac0237d01b158fd3f0d3f93a0f90559376d`  
		Last Modified: Wed, 12 Jan 2022 16:05:03 GMT  
		Size: 189.3 MB (189319899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1e048a3d0afbdd624a6f302868219c29f7bfb0784ada830d3d276e7c0ac6b8`  
		Last Modified: Wed, 12 Jan 2022 16:01:38 GMT  
		Size: 311.0 KB (310954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
