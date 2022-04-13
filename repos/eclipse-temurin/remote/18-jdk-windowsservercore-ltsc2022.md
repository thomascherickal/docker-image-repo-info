## `eclipse-temurin:18-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:8adaa7c60abf6aae61ae52db98cb16d8c5b899b1927223da587a4d4fa534dc46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `eclipse-temurin:18-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:06aa7df179c5f7c7c5f13c285b57c071ee1f8bfac0db5a0e846575c8afd36a9f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2582233919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d2ed0a5549657e973167b9f02a2af4ee2fdda2b878254ec9fe3d54b827bc12`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 15:42:36 GMT
ENV JAVA_VERSION=jdk-18+36
# Wed, 13 Apr 2022 15:43:38 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_x64_windows_hotspot_18_36.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_x64_windows_hotspot_18_36.msi ;     Write-Host ('Verifying sha256 (28280dd5453a252d412894c9a5b5bcf84ea426a9ecc20135f791f3875b73f343) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '28280dd5453a252d412894c9a5b5bcf84ea426a9ecc20135f791f3875b73f343') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-18' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Apr 2022 15:44:03 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 13 Apr 2022 15:44:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87cca2d60b3679e815f3998b2aec26adb91b5dede2bc8152090af883d5b3be8`  
		Last Modified: Wed, 13 Apr 2022 16:30:35 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3832afa047d20e7c17d9ecc4060e98090e19d679049b5a2706c747353ac9984a`  
		Last Modified: Wed, 13 Apr 2022 16:37:04 GMT  
		Size: 354.7 MB (354698603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e4642521eaa60a199a728518e0d9d1a4fdde2842b348409f7d8b8edaa41752`  
		Last Modified: Wed, 13 Apr 2022 16:30:36 GMT  
		Size: 576.2 KB (576185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f714a105dc92e1d0ad2c101b7f2981f3bffc2e91ff9b69e71015edefefcf64`  
		Last Modified: Wed, 13 Apr 2022 16:30:36 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
