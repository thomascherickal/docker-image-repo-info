## `eclipse-temurin:8-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:926b88089daff22eb8f9571bce7c3fba43c95631f2553d3ac1b2a2a10391abca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:8-jdk-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull eclipse-temurin@sha256:55f755f90f164df9a50695f0de2c2bba1bbc8c40bb28642426064564efb47917
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2251641696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f53c31f02016ff2b6964504e95283a3483920af56e0560b966d7f052b5ac5ee`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 00:11:39 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Wed, 13 Dec 2023 00:13:12 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_windows_hotspot_8u392b08.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u392-b08/OpenJDK8U-jdk_x64_windows_hotspot_8u392b08.msi ;     Write-Host ('Verifying sha256 (223d252802b9087e85886f08faebf9fa676285565895e74ec2f9bde4b1f39f03) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '223d252802b9087e85886f08faebf9fa676285565895e74ec2f9bde4b1f39f03') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Dec 2023 00:14:21 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:9e0ea737a451ed64b01ce3e4786ce81de3316152dc4c1569b4710cd8f60f660d`  
		Last Modified: Wed, 13 Dec 2023 06:34:38 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b202125861105899c7ead391bef127a02d12fc466c0996dae7a319648ee39e74`  
		Last Modified: Wed, 13 Dec 2023 06:34:54 GMT  
		Size: 191.6 MB (191643775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4736cc1e48005083651f4160294c84ca18545f541153ae42d4faeb0e83236f26`  
		Last Modified: Wed, 13 Dec 2023 06:34:39 GMT  
		Size: 286.2 KB (286172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
