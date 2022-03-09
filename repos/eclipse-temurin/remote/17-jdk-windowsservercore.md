## `eclipse-temurin:17-jdk-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:3da6be9d8ab74a3c3557319a6773a3a18f565f6f4e3d8e52be0740193c37e687
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `eclipse-temurin:17-jdk-windowsservercore` - windows version 10.0.20348.587; amd64

```console
$ docker pull eclipse-temurin@sha256:e33d762a6c7eb909f1cd81180b9d394e8dd93fc7249e7f79d76b1c8b3f0610b8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2574310171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86832beb3b6dba606852956cb7f9f9f54e3188e6da9f207038c0fcd3531f2d14`
-	Default Command: `["jshell"]`
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
# Tue, 08 Mar 2022 22:17:00 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_x64_windows_hotspot_17.0.2_8.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_x64_windows_hotspot_17.0.2_8.msi ;     Write-Host ('Verifying sha256 (f66f21f0b25e4fe0449c41555dbeb7ba890d54e5a6e48e35b1a6309409eaf2d1) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f66f21f0b25e4fe0449c41555dbeb7ba890d54e5a6e48e35b1a6309409eaf2d1') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Tue, 08 Mar 2022 22:17:25 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Tue, 08 Mar 2022 22:17:26 GMT
CMD ["jshell"]
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
	-	`sha256:43e82078215b9090db5dea38f0c1caa9bcace0049dc2724048081b854b7fe257`  
		Last Modified: Tue, 08 Mar 2022 22:49:03 GMT  
		Size: 352.5 MB (352533642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea88bce5da437c7f0c3224adf4a6eac67755a13831457e58337f3561865dc4b`  
		Last Modified: Tue, 08 Mar 2022 22:48:33 GMT  
		Size: 525.3 KB (525254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045e7e8a63823f28342761f97cfa76418a0b6d934eddcaf0f3abd727ef2d8700`  
		Last Modified: Tue, 08 Mar 2022 22:48:32 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull eclipse-temurin@sha256:a8bd4598e34609275f14dcefa251a0a916149a5d60db805b73c8767a59d29a35
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3071662248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1b9a40e1984ab12d81c0ca13e7184aa53293842660a6c6c37aafd8676086ade`
-	Default Command: `["jshell"]`
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
# Tue, 08 Mar 2022 22:19:26 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_x64_windows_hotspot_17.0.2_8.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_x64_windows_hotspot_17.0.2_8.msi ;     Write-Host ('Verifying sha256 (f66f21f0b25e4fe0449c41555dbeb7ba890d54e5a6e48e35b1a6309409eaf2d1) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f66f21f0b25e4fe0449c41555dbeb7ba890d54e5a6e48e35b1a6309409eaf2d1') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Tue, 08 Mar 2022 22:20:27 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Tue, 08 Mar 2022 22:20:28 GMT
CMD ["jshell"]
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
	-	`sha256:d6d32154fac7158cd90aba758fd97e649db9500eb69f48af3235092293af4647`  
		Last Modified: Tue, 08 Mar 2022 22:49:48 GMT  
		Size: 352.3 MB (352320452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163957be1d2b2275a421fa9f24a97142e2fe8b3112b5549f9620bb23ed618fb2`  
		Last Modified: Tue, 08 Mar 2022 22:49:18 GMT  
		Size: 3.9 MB (3885047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19be536239aab380677e65e03c339e678c6c7d9370168f57673c9f6325dc8b77`  
		Last Modified: Tue, 08 Mar 2022 22:49:16 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
