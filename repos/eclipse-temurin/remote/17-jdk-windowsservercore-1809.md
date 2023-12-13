## `eclipse-temurin:17-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:e7a4b94570b033ed76fda71c27b26f2531dc4a9fc3d8640b97d9a66ba538801b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:17-jdk-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull eclipse-temurin@sha256:181018e090e0c12a1eab94777aa69a78df790cb733e9d562c2794510e06c4f86
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2418518925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd9bcbd4ed6167b9c32a56a3ec1c544f50edc0bf548a0ffc597dcce0f840d029`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 00:30:46 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Wed, 13 Dec 2023 00:32:22 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9.1/OpenJDK17U-jdk_x64_windows_hotspot_17.0.9_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9.1/OpenJDK17U-jdk_x64_windows_hotspot_17.0.9_9.msi ;     Write-Host ('Verifying sha256 (cd7b319f6fbd7efc68a0e464c55c7f2a28d6b8be3d0bcda315a16f885c57cadb) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'cd7b319f6fbd7efc68a0e464c55c7f2a28d6b8be3d0bcda315a16f885c57cadb') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Dec 2023 00:33:38 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 13 Dec 2023 00:33:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e713f7a8c8573f151ea720fd00ac2cc49d48a16f6cf310f6d99bf99ead3774`  
		Last Modified: Wed, 13 Dec 2023 06:39:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056c274dfd2f30930a883b7ed8b63f849d9c1128e788af20b95c54d06a26a1c1`  
		Last Modified: Wed, 13 Dec 2023 06:39:53 GMT  
		Size: 355.0 MB (355001453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f33be3315c8e397a75315e5a62a4f7b09fed8c72c1e85e7f26c7bbe28b93991`  
		Last Modified: Wed, 13 Dec 2023 06:39:29 GMT  
		Size: 3.8 MB (3804419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e68f9f87d140b0074403f5a143f5019f486d21912391cb0c26f8fafee2d883`  
		Last Modified: Wed, 13 Dec 2023 06:39:28 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
