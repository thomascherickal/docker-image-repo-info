## `eclipse-temurin:8u312-b07-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:8bc8c27f7088da7d32474af1320975596ec0d013602b3269d483376fafb2010c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.350; amd64

### `eclipse-temurin:8u312-b07-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.350; amd64

```console
$ docker pull eclipse-temurin@sha256:1e4940975c19db7b55d33d93d8168182e075b2058c3eb05fe5619e8d4c0bdf47
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2374726593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:025a2aad3e3cd4208ecfcdf1c4b64db4fa3ab7c6be73b98c9e3b838547b2f5cb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 03 Nov 2021 08:36:33 GMT
RUN Install update ltsc2022-amd64
# Wed, 10 Nov 2021 01:38:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 17:09:26 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 10 Nov 2021 17:10:13 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_windows_hotspot_8u312b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_windows_hotspot_8u312b07.msi ;     Write-Host ('Verifying sha256 (5544ebcb03206f3c3f5f19f6da03003a154cb2b489a06d88a052792f72b76c21) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '5544ebcb03206f3c3f5f19f6da03003a154cb2b489a06d88a052792f72b76c21') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Nov 2021 17:10:39 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0eb404f1860fa8786ad09d1d9fe9fd580115f83cd38623bc4eb0c46abdaa0a3`  
		Size: 932.9 MB (932907933 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:27ded59d7006d9d7bffa7c253cd04a900a5d6b0d47b84d0edd624d12fd64cdc9`  
		Last Modified: Wed, 10 Nov 2021 02:07:39 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beb5d53c7742662204cb4553961c377c0700c758d5917e271258e09714ca3f2`  
		Last Modified: Wed, 10 Nov 2021 17:57:45 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f618a46b0b0cc825ce459c3ce789d01caecaf81ccf4409e1536d8057727a2c`  
		Last Modified: Wed, 10 Nov 2021 18:01:15 GMT  
		Size: 189.6 MB (189553877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e97612f48dd546b5d872b1783e5b410136a0469997e15ec0b708c4ef8b22fd`  
		Last Modified: Wed, 10 Nov 2021 17:57:46 GMT  
		Size: 562.9 KB (562901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
