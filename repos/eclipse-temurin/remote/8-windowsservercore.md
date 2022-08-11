## `eclipse-temurin:8-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:70672d507c6df72ef7439cf4ac027a4eb2c08e93635a07cda56ba2bd758350ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `eclipse-temurin:8-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull eclipse-temurin@sha256:18f789463254c8bc5e7a97a638ea547a861abfc4d75303a502c2eeeae3a9ef55
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2507548964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2204a43dff250bbc038fb64404649865cbbcd506745431922c25ec3fb20c72c0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 11 Aug 2022 19:15:23 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 11 Aug 2022 19:16:21 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u345b01.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u345b01.msi ;     Write-Host ('Verifying sha256 (a19b85fedcc830aa81c6aeb07449905032b7b391c033a1647639486b25f2e1f3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'a19b85fedcc830aa81c6aeb07449905032b7b391c033a1647639486b25f2e1f3') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Thu, 11 Aug 2022 19:16:51 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e0e2dd6d67f1b8ed30ce1606e5716fed6ccb4320f91d2f508ce1a6c4275461`  
		Last Modified: Thu, 11 Aug 2022 19:31:11 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c861b4e8b511548190be462fd3a60ec168f9fa5b0e4cd6eacee159663982799d`  
		Last Modified: Thu, 11 Aug 2022 19:31:27 GMT  
		Size: 190.1 MB (190087230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b901e41f1122821becf90341d37698201f60e642135568176b526943b410134`  
		Last Modified: Thu, 11 Aug 2022 19:31:11 GMT  
		Size: 569.7 KB (569741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull eclipse-temurin@sha256:c4be55ec261a0555a1ec8b171b132fde6a21bd3510ca46fb3500c3ad13000c70
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2867863004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:683cfe32e5c7c4eea092e112edeec13acaaae5be737e213b7b804ea97a6c0932`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 11 Aug 2022 19:17:10 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 11 Aug 2022 19:18:54 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u345b01.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u345b01.msi ;     Write-Host ('Verifying sha256 (a19b85fedcc830aa81c6aeb07449905032b7b391c033a1647639486b25f2e1f3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'a19b85fedcc830aa81c6aeb07449905032b7b391c033a1647639486b25f2e1f3') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Thu, 11 Aug 2022 19:20:03 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d875e078fae7eb20d0fb76130e2e165680c4a1f38e86ef8fe0b2ed27f02b7c`  
		Last Modified: Thu, 11 Aug 2022 19:31:40 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94fc0ee34fb6dcb20a1dd70e413c93dab7e15537d4e38bb6cefeed4696d35ea`  
		Last Modified: Thu, 11 Aug 2022 19:31:57 GMT  
		Size: 189.8 MB (189830748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912ed8170caff5789bb377cfc0ad679e16489f95cd46ee38d9a022ebb218b620`  
		Last Modified: Thu, 11 Aug 2022 19:31:40 GMT  
		Size: 316.7 KB (316672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
