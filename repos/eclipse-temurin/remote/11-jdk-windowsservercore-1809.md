## `eclipse-temurin:11-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:ef8946dc7cac4741da4d65c9c16852734b7a1da07da02291f91a189440115b64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:11-jdk-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:d025044f692c9759f65e35065cea86107ea4839374f54c7ecbfedd28d8d29751
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2018072445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bcd1686bf38e31805963e92a544bdcb53dc777f0d79e24a78bcd808d5989d9b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 00:47:16 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Sat, 24 Jun 2023 00:48:18 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_x64_windows_hotspot_11.0.19_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_x64_windows_hotspot_11.0.19_7.msi ;     Write-Host ('Verifying sha256 (8f8f136e2071591c6ea7bc58d629a5c8ad23c829bb1878200fdff0c0fe97712c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8f8f136e2071591c6ea7bc58d629a5c8ad23c829bb1878200fdff0c0fe97712c') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 24 Jun 2023 00:48:45 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Sat, 24 Jun 2023 00:48:46 GMT
CMD ["jshell"]
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
	-	`sha256:5d33d388117795a20af7fd950480a084fa7e10b50eeed7da58414e6b32fb793a`  
		Last Modified: Sat, 24 Jun 2023 01:26:44 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b02f352863201370822135eeee68c8816b9b140540bbfe2ccb3c42c65a42a94`  
		Last Modified: Sat, 24 Jun 2023 01:27:12 GMT  
		Size: 367.1 MB (367065623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6427ae7e7524f08e8c2dfe85caed0178e307928ae19c7463f9935dd45d3006bb`  
		Last Modified: Sat, 24 Jun 2023 01:26:44 GMT  
		Size: 266.0 KB (266026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1e6816a38a18ce8202ac53b24f1b5e49d058982736615ef4dc6370a4ffc09d`  
		Last Modified: Sat, 24 Jun 2023 01:26:44 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
