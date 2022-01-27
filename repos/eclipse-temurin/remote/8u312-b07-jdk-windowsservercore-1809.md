## `eclipse-temurin:8u312-b07-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:826d427bcbfb35405a6fc4bd898cdf65ea76292fa6276beeda4eb5b8377de811
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:8u312-b07-jdk-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:1b084e1ef71000abcf81f86024bdf6ca18c3fa80959427db36c8249204fc440d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2903013128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fced9cda5189134d08b25cfa9ed30623686a6f83aece2b567b459c1b227a4a82`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 19:00:34 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 26 Jan 2022 19:02:26 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_windows_hotspot_8u312b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_windows_hotspot_8u312b07.msi ;     Write-Host ('Verifying sha256 (5544ebcb03206f3c3f5f19f6da03003a154cb2b489a06d88a052792f72b76c21) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '5544ebcb03206f3c3f5f19f6da03003a154cb2b489a06d88a052792f72b76c21') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 26 Jan 2022 19:03:37 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8c9a9ad30800bb1daff963b295ab56fd35420694be2ba090fd7d99d827f90e`  
		Last Modified: Wed, 26 Jan 2022 19:51:37 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2da924cbe5b609be4c082b4a4564b08fafdd20794415ed90ef9b7e3f0460323`  
		Last Modified: Wed, 26 Jan 2022 19:55:22 GMT  
		Size: 189.4 MB (189351888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ce087c4b8381f4ce1714c69e29bfee235628ffa103e905b41dc2f62adac6da`  
		Last Modified: Wed, 26 Jan 2022 19:51:37 GMT  
		Size: 336.9 KB (336906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
