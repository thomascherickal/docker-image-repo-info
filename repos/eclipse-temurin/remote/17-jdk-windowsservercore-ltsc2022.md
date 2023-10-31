## `eclipse-temurin:17-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:8ba951a5697d520c73ef40490695b967b813a6776f528376580b631ed0e3cc6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `eclipse-temurin:17-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:2246350ce512ffccd5583ed243b0b809ca7f464fc5c599bfdbc13923cfd2afe3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2215111707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a1ba84902cbad29162441118d5796e8a6403c0c4161f4e116f3d08b7054d36d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 30 Oct 2023 23:24:30 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:25:23 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9.1/OpenJDK17U-jdk_x64_windows_hotspot_17.0.9_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9.1/OpenJDK17U-jdk_x64_windows_hotspot_17.0.9_9.msi ;     Write-Host ('Verifying sha256 (cd7b319f6fbd7efc68a0e464c55c7f2a28d6b8be3d0bcda315a16f885c57cadb) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'cd7b319f6fbd7efc68a0e464c55c7f2a28d6b8be3d0bcda315a16f885c57cadb') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 30 Oct 2023 23:25:48 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Mon, 30 Oct 2023 23:25:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16153d3285bf0ec2e836bd1b1232717379207b06fccb57f2403fb4833d496b6`  
		Last Modified: Mon, 30 Oct 2023 23:50:15 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bb1d80389f0ea2b716bd9141aa562d57d56b2c60bf90044aae64e24844b9ea`  
		Last Modified: Mon, 30 Oct 2023 23:50:38 GMT  
		Size: 355.0 MB (354975287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d4309ace962dc15043315a098bf52e6e40c4d9514e5d5f901d30c485bec249`  
		Last Modified: Mon, 30 Oct 2023 23:50:15 GMT  
		Size: 289.1 KB (289132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845b77db9d3515131a432c660e41eef292641cbc15a7550726d972a5075b5466`  
		Last Modified: Mon, 30 Oct 2023 23:50:15 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
