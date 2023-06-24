## `eclipse-temurin:8u372-b07-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:ac5b365586741c235525a949827b3de5313460f7cee51a72f81e8e7d4d5d9010
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:8u372-b07-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:dac223f32e09cc127978fa2ec72215e48dd4cbea240b822efd8baf90bf0bd849
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1617660379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f8dfae35683700a3b4a982e25929f91751870977e4bc722ccf3ca5ba70d68ff`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 00:38:08 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Sat, 24 Jun 2023 00:39:15 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_x64_windows_hotspot_8u372b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_x64_windows_hotspot_8u372b07.msi ;     Write-Host ('Verifying sha256 (e75a4e4a70d0fb5c0f1ca4855cb2a7f3c9ccb3d5dea5af0f45d4608a563c45b8) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e75a4e4a70d0fb5c0f1ca4855cb2a7f3c9ccb3d5dea5af0f45d4608a563c45b8') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 24 Jun 2023 00:39:47 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87ee159de2b83674325425f18750af6017f5eb28e3112293ec457fdef5c16dd`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e9771550f15b9ae9cb9acd578a751ca317ea17381d029c276b6299b87164dc`  
		Last Modified: Sat, 24 Jun 2023 01:16:17 GMT  
		Size: 191.1 MB (191071693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699b6daf63321c9df57f126e47d04b2b7ec1f91bc83d356034e5e919d9171e0c`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 287.3 KB (287328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
