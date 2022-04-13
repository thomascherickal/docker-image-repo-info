## `eclipse-temurin:11-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:30b20ff6b8c3d6cd74492b3f0ef19256fd945fb9cc24443224e63edc32dd4362
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `eclipse-temurin:11-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:7134c627108fc2e236946ec22a452431f5e3f62bc7358300c4e80375d5bd08a0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2593786171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c89ff5e138cb586049313182e41bd14b74e9d0e7d69222b85869d60f8b8702a4`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 15:20:23 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Wed, 13 Apr 2022 15:21:25 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_windows_hotspot_11.0.14.1_1.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_windows_hotspot_11.0.14.1_1.msi ;     Write-Host ('Verifying sha256 (afa6379e9b4bab0bdbf40a1051a219414d8c8fcb2c095e1552d23505293a577e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'afa6379e9b4bab0bdbf40a1051a219414d8c8fcb2c095e1552d23505293a577e') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Apr 2022 15:21:48 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 13 Apr 2022 15:21:49 GMT
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
	-	`sha256:36b482e92bae944bf348048ca1c910ad10e42da6b29eb83155e0882d2a67c04f`  
		Last Modified: Wed, 13 Apr 2022 16:02:30 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae871eabb87adda592be082b9f4924dc1387c103e2861754fcb5bd612313a85`  
		Last Modified: Wed, 13 Apr 2022 16:08:52 GMT  
		Size: 366.3 MB (366251446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217b32f5bff8799f86501e837e7999718a320a851ce170b35954408b4a513598`  
		Last Modified: Wed, 13 Apr 2022 16:02:30 GMT  
		Size: 575.7 KB (575734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9126e3d80c9a05f6c3c1f1cf3557a37ac860c7d792c574abf368114c04023`  
		Last Modified: Wed, 13 Apr 2022 16:02:30 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
