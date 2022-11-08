## `eclipse-temurin:17-jdk-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:dce6bfa7ece7405ebe825f8318f7bcefc1d770c8c711aadc2028c32894719a1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1129; amd64
	-	windows version 10.0.17763.3532; amd64

### `eclipse-temurin:17-jdk-windowsservercore` - windows version 10.0.20348.1129; amd64

```console
$ docker pull eclipse-temurin@sha256:3334dded755982468d05992497f648b037ffd61592639fca6151e04c585ec6f6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2827290826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0069d8db61926c278d242cadcdfc21198131c8637a92d03d7ad382c79e1438a1`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 07 Nov 2022 20:15:53 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 20:17:21 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_x64_windows_hotspot_17.0.5_8.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_x64_windows_hotspot_17.0.5_8.msi ;     Write-Host ('Verifying sha256 (33a2d3d25d83cc6c7e5e7267bfa4c262319555f402d771ce1e05abbf52183391) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '33a2d3d25d83cc6c7e5e7267bfa4c262319555f402d771ce1e05abbf52183391') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 07 Nov 2022 20:17:52 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Mon, 07 Nov 2022 20:17:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e237f26265172bc7812832923fde755cee3451453c14654b05966871fcdd677b`  
		Last Modified: Mon, 07 Nov 2022 20:34:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276582988c0e9562253e3ac3d803553cc326ec6a7d7c72e644259a62433897ac`  
		Last Modified: Mon, 07 Nov 2022 20:34:39 GMT  
		Size: 352.7 MB (352709871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfb889ef4df8911e58a6d71f07b08d2ff3bfda7e509008947993b48028de11c`  
		Last Modified: Mon, 07 Nov 2022 20:34:05 GMT  
		Size: 550.4 KB (550382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8229617f18ed3342b870361e16fe401c6fd3c012f893eb750053fad64d4adf62`  
		Last Modified: Mon, 07 Nov 2022 20:34:04 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull eclipse-temurin@sha256:bbc478aaef858536139166eb7691bfb261d1ec894f194b090e4405e61e74e50a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3129893669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b5ac294cb4e20b073916fd4daf5a97abc9f64ee0559671a1acd415902fd265`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 07 Nov 2022 20:18:10 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 20:20:32 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_x64_windows_hotspot_17.0.5_8.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_x64_windows_hotspot_17.0.5_8.msi ;     Write-Host ('Verifying sha256 (33a2d3d25d83cc6c7e5e7267bfa4c262319555f402d771ce1e05abbf52183391) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '33a2d3d25d83cc6c7e5e7267bfa4c262319555f402d771ce1e05abbf52183391') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 07 Nov 2022 20:21:48 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Mon, 07 Nov 2022 20:21:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76354ece1c888d04cec9980bde3c3c4a2446905638dd11bbc97598943f733001`  
		Last Modified: Mon, 07 Nov 2022 20:34:52 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd196d74b3efbecf668feb38edacba2f6ff1e9e2bc654b3782bfc175257c194`  
		Last Modified: Mon, 07 Nov 2022 20:35:28 GMT  
		Size: 352.5 MB (352486146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08153eeb63ef612256edf8bf06ddd59b840e756d3ac87421a0daa0c8c089a335`  
		Last Modified: Mon, 07 Nov 2022 20:34:54 GMT  
		Size: 3.9 MB (3904901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54eb817d2632a76b4f98d4028e2018508bc8103b3bafd811381bbd75c266418`  
		Last Modified: Mon, 07 Nov 2022 20:34:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
