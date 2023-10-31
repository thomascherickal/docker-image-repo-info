## `eclipse-temurin:17-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:c78fd54e6e4e7e893b650c60b562ec8206218d76500afc73c48bcff974784ab9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:17-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:7979ca9474605be958283a27c95e913b1293da4c97d5da37f36dae0ee9d9e3ed
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2390404383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aedc367e9ecb41485313ba2aae86c04e5adb6c034ae5b01188fa0a0c7a578f46`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 30 Oct 2023 23:25:59 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:27:27 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9.1/OpenJDK17U-jdk_x64_windows_hotspot_17.0.9_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9.1/OpenJDK17U-jdk_x64_windows_hotspot_17.0.9_9.msi ;     Write-Host ('Verifying sha256 (cd7b319f6fbd7efc68a0e464c55c7f2a28d6b8be3d0bcda315a16f885c57cadb) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'cd7b319f6fbd7efc68a0e464c55c7f2a28d6b8be3d0bcda315a16f885c57cadb') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 30 Oct 2023 23:28:27 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Mon, 30 Oct 2023 23:28:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ca572b33dd9ed62ebb25ce3227b33eaa39cee409c4b93e18bc256aeb3d05fe`  
		Last Modified: Mon, 30 Oct 2023 23:50:52 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a432086e6c7ff3a165bab8958e280995f3bb9644e1578fdfa98bbe456f98db55`  
		Last Modified: Mon, 30 Oct 2023 23:51:16 GMT  
		Size: 355.0 MB (355003278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d51bcd49b30a18cea9afcf770c8aa97774e052d9b44151f1646e7bf7a545c2`  
		Last Modified: Mon, 30 Oct 2023 23:50:53 GMT  
		Size: 3.8 MB (3806484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd048baec27fdf6fc36deef4b8cba908816d3f935a361a3f61693ad796fcb4db`  
		Last Modified: Mon, 30 Oct 2023 23:50:52 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
