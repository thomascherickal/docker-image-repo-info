## `eclipse-temurin:8u322-b06-jre-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:8ca4a0ff7a1b72bc8923e71c01be1f6ad30461013a6ea37ce3722a7a5043dbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.643; amd64
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:8u322-b06-jre-windowsservercore` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:f8ad347ffd12c1350810c2c8bd94ede3f6021d0ce0a463104b6ea1f857068581
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2298441907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fd0056aba17a339d4e78f63904e18b82039333e270180cd7755c693199bc128`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 15:12:15 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Wed, 13 Apr 2022 15:17:22 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_windows_hotspot_8u322b06.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_windows_hotspot_8u322b06.msi ;     Write-Host ('Verifying sha256 (74eb66d2d6aefdc42f95681616c94f6a41b1e133d899131719cf8c2f0cbf0a25) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '74eb66d2d6aefdc42f95681616c94f6a41b1e133d899131719cf8c2f0cbf0a25') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Apr 2022 15:17:42 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:c8f928df4aebcabe565eb4cb6d5dbbf1ac28479dac45dbdfc3b86d72daaed813`  
		Last Modified: Wed, 13 Apr 2022 15:54:03 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab434ffd135ddf5af18fe93e1ad179804267075ef210d9abb3a5d5e82be3729`  
		Last Modified: Wed, 13 Apr 2022 16:01:45 GMT  
		Size: 70.9 MB (70907466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d6b46a5fa5bbc83919aa67f1dd953eff5ba5eeb337cd8e2132b8e4a073b700`  
		Last Modified: Wed, 13 Apr 2022 16:00:28 GMT  
		Size: 576.9 KB (576852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u322-b06-jre-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:3713558fe149d47e3fd821087587799f9edf8b375a3b4f5715ca8dc01720e0ef
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2786933541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af6c51c72394eda897f926b1856110c917331c59f94530b723df64c6e2f29248`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 15:13:43 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Wed, 13 Apr 2022 15:18:53 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_windows_hotspot_8u322b06.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_windows_hotspot_8u322b06.msi ;     Write-Host ('Verifying sha256 (74eb66d2d6aefdc42f95681616c94f6a41b1e133d899131719cf8c2f0cbf0a25) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '74eb66d2d6aefdc42f95681616c94f6a41b1e133d899131719cf8c2f0cbf0a25') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Apr 2022 15:19:46 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda3f8877932a5001b8f1e44d7fc68f233d50da7e29742e9b26a24f99f161fd`  
		Last Modified: Wed, 13 Apr 2022 15:57:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d74aa6195c10f0e3f150c132f17e76d5664e02a1063b6d1f6840937249e68ed`  
		Last Modified: Wed, 13 Apr 2022 16:02:03 GMT  
		Size: 70.7 MB (70678796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286eec6204017a1ae9abff3885663798ef6a2f9ad6eaad3ddfd390a984f109e4`  
		Last Modified: Wed, 13 Apr 2022 16:01:56 GMT  
		Size: 331.7 KB (331710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
