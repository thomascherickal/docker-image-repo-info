## `eclipse-temurin:18-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:e92e98f79cb7d0d2025ce1de453dfb2b8a5738ac5740989d0ac3f9d4e90a41c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `eclipse-temurin:18-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull eclipse-temurin@sha256:a6ffceadff0562ad4dcd578525bdf98fc126a86f72349ba0589f38d712a8af7b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2672630439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12da9308266f16b4bda550941dce533e114359b4188aecbf785308db582e7c5a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 29 Aug 2022 18:17:59 GMT
ENV JAVA_VERSION=jdk-18.0.2.1+1
# Mon, 29 Aug 2022 18:19:34 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2.1%2B1/OpenJDK18U-jdk_x64_windows_hotspot_18.0.2.1_1.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2.1%2B1/OpenJDK18U-jdk_x64_windows_hotspot_18.0.2.1_1.msi ;     Write-Host ('Verifying sha256 (e766c2d6100e70786ff0bb154054dd64bb45ea14ffc995544bbced98eb1c8703) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e766c2d6100e70786ff0bb154054dd64bb45ea14ffc995544bbced98eb1c8703') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-18' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 29 Aug 2022 18:20:04 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Mon, 29 Aug 2022 18:20:06 GMT
CMD ["jshell"]
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
	-	`sha256:59057329e6b2bd10b8538e422dd37bfba432b4c7c59703943787dc793140fa15`  
		Last Modified: Mon, 29 Aug 2022 18:34:22 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0dfcae41964f6e70c5161ab95895a061c61e2914cecc3b7ec793e8f13ec783a`  
		Last Modified: Mon, 29 Aug 2022 18:34:51 GMT  
		Size: 355.2 MB (355155341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bbb160c4affae37d08969dfd30ace2b417fca082fb02e05fe4588c99d3456d`  
		Last Modified: Mon, 29 Aug 2022 18:34:22 GMT  
		Size: 581.7 KB (581711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7229bbdeede41f775caefcfc7ccc4559c696dc35f639cf44fda94057bbf7e883`  
		Last Modified: Mon, 29 Aug 2022 18:34:22 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
