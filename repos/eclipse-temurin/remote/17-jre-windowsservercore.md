## `eclipse-temurin:17-jre-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:0fe47073e71d28e0f67ad78d3c27fc20019e68067317b73df2d97d1d7392d256
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `eclipse-temurin:17-jre-windowsservercore` - windows version 10.0.20348.587; amd64

```console
$ docker pull eclipse-temurin@sha256:db65483f64ed5a7e8d226b9fa2c8219661e130501f0f82a8948b389b5df56c44
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2296193857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd2daf79bc31cf73e5a727ac47f12d8c7b0ed6f4426843bc9a58d61840b2bb13`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Mar 2022 22:15:41 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Tue, 08 Mar 2022 22:22:15 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_windows_hotspot_17.0.2_8.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_windows_hotspot_17.0.2_8.msi ;     Write-Host ('Verifying sha256 (57c39a19ba3fb5c17cee620a9f5437f73e12034efb70a9e3d9bd621a1b5e852b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '57c39a19ba3fb5c17cee620a9f5437f73e12034efb70a9e3d9bd621a1b5e852b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Tue, 08 Mar 2022 22:22:38 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd2d1753acc9962f9bb2576c33821db5bfc56fc0a7805b27cc6351c9cd3fa12`  
		Last Modified: Tue, 08 Mar 2022 22:48:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ab1620192aed3814de8656523e9489c9b983545f1d5436c4b6cee7886a285a`  
		Last Modified: Tue, 08 Mar 2022 22:55:24 GMT  
		Size: 74.4 MB (74418760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d62ea2077695df2a3d19885f6837debc7ea3a49f87bcbad89d1fcf5628d1fad`  
		Last Modified: Tue, 08 Mar 2022 22:53:56 GMT  
		Size: 525.2 KB (525215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull eclipse-temurin@sha256:6f584c5707d4bfad2e842d436de98b439f296ed5b95f32358f841201a9dbf742
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2792916705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:820c09c1837aabe49f85378327802268185b0165981ac14483d8a7675a7cdb4a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Mar 2022 22:17:41 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Tue, 08 Mar 2022 22:24:03 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_windows_hotspot_17.0.2_8.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_windows_hotspot_17.0.2_8.msi ;     Write-Host ('Verifying sha256 (57c39a19ba3fb5c17cee620a9f5437f73e12034efb70a9e3d9bd621a1b5e852b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '57c39a19ba3fb5c17cee620a9f5437f73e12034efb70a9e3d9bd621a1b5e852b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Tue, 08 Mar 2022 22:25:13 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e224724b1d5c532011fd45aa7e9afea1981b72cbe9a7e6de274eddbac57f904`  
		Last Modified: Tue, 08 Mar 2022 22:49:16 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcce31a5820f9aec17a205957892a672d57a15713f77633db1c3ff6427806ef`  
		Last Modified: Tue, 08 Mar 2022 22:57:03 GMT  
		Size: 74.2 MB (74192862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25977283632929199005a74efa07727ba0b2424bce06d958e6ec32a9be658d07`  
		Last Modified: Tue, 08 Mar 2022 22:55:35 GMT  
		Size: 3.3 MB (3268479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
