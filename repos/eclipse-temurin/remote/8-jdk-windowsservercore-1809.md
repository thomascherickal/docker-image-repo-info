## `eclipse-temurin:8-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:ecb62d320c41e13740c192c3e75d548ab5b3e354aafe4c445c52f8c4137a269a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:8-jdk-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:8a033d87542035165314f1de89f81cbc8d8aa27c4253031b89db72e94cc6dfea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1842102062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cacffd59006466cb65670e3dd26b51b951c680f817044d4808556ff019e7907`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 00:40:08 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Sat, 24 Jun 2023 00:41:10 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_x64_windows_hotspot_8u372b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_x64_windows_hotspot_8u372b07.msi ;     Write-Host ('Verifying sha256 (e75a4e4a70d0fb5c0f1ca4855cb2a7f3c9ccb3d5dea5af0f45d4608a563c45b8) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e75a4e4a70d0fb5c0f1ca4855cb2a7f3c9ccb3d5dea5af0f45d4608a563c45b8') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 24 Jun 2023 00:41:40 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:da248a958935c5b8ee2bbb701b9491c5775a0ad49b5d958119ae6414f9b72e45`  
		Last Modified: Sat, 24 Jun 2023 01:20:22 GMT  
		Size: 191.1 MB (191084263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ec0aca2730fb5b8910c9f16e5353ce8cd8b79c78a85b249171329e06f0bc6`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 278.2 KB (278172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
