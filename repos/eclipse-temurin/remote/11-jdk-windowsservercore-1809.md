## `eclipse-temurin:11-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:58a414f950507b99cef747e66f3d40885185c5a530ace5cca5d39d52923f7e11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:11-jdk-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull eclipse-temurin@sha256:3bb63ca8fee16e74caaa2e358ea266a076b152b0e7480fec5a471d502080019c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2429148177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c88cd63979664f42419929b9c3e34a2b084754400a1dc8e4a1ec8b143eb5a0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 00:21:15 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 13 Dec 2023 00:22:53 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.21_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.21_9.msi ;     Write-Host ('Verifying sha256 (ccaa09811f488cf95340e2702e8d9176058a52e89808ae6e1a1d20de39e5ce34) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'ccaa09811f488cf95340e2702e8d9176058a52e89808ae6e1a1d20de39e5ce34') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Dec 2023 00:23:58 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 13 Dec 2023 00:23:59 GMT
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
	-	`sha256:22613c8f55cb8faa07b5c958077cfbefb515e8040ee3f5f8d4c23a6b9c85a5ec`  
		Last Modified: Wed, 13 Dec 2023 06:36:52 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e065aa6f33926f10e0734001109a6fd1d16f004cd82e04f83307ec384ae76d05`  
		Last Modified: Wed, 13 Dec 2023 06:37:18 GMT  
		Size: 369.1 MB (369148499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f5bf6e7572a5553920e254264b5ed338542218d5e10dd83845060e0778cd98`  
		Last Modified: Wed, 13 Dec 2023 06:36:52 GMT  
		Size: 286.7 KB (286732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4882915a066592db64632cfeaf0305c605c6951df3df0a267ca79a60657a471`  
		Last Modified: Wed, 13 Dec 2023 06:36:52 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
