## `eclipse-temurin:20-jre-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:f5944a602c5530461cc3e9067c907b6dd3ec406bc1c64fdd7d6961efe656e1be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:20-jre-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:ab0a0c0e3bbd744788d12f8d24b0f48aa0a21ae07529c50dbeed827675a6bb3b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1732447228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d47d7bcd60044c17dc0561b61af1a3fe920e021472007ee2a0fb247cefb89af`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 01:02:19 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Sat, 24 Jun 2023 01:06:57 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ;     Write-Host ('Verifying sha256 (2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-20' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 24 Jun 2023 01:07:27 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
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
	-	`sha256:83cc725e51be377d486df843039f1371f7e90bc8e29500b65bf085b11bb56247`  
		Last Modified: Sat, 24 Jun 2023 01:32:12 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8fe5a8a0ba9db4a11398eb6c6f9e34660f149e1dcbd6b8e3ce0c2ada53509e`  
		Last Modified: Sat, 24 Jun 2023 01:33:54 GMT  
		Size: 78.4 MB (78385518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e14e24dd4591557a3d0ff1e49a3086dca539e7a04660dec361d87347a30494`  
		Last Modified: Sat, 24 Jun 2023 01:33:44 GMT  
		Size: 3.3 MB (3322098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
