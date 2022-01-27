## `eclipse-temurin:8u312-b07-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:f8a953d00ed88220d5e01149379abcf0d3c3f1a11ffa7c9dd217410b90438d90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.473; amd64

### `eclipse-temurin:8u312-b07-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.473; amd64

```console
$ docker pull eclipse-temurin@sha256:6807bc283e05d7dcceb15c281d0f3d636e638b6ccde741ed9feaa79a88e0a596
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2278871711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8af01cb13caa65b6983328651e56509171153a6c7109d1e0616e2666be490051`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 16 Jan 2022 05:17:24 GMT
RUN Install update ltsc2022-amd64
# Wed, 19 Jan 2022 22:21:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 18:58:21 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 26 Jan 2022 19:05:38 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_windows_hotspot_8u312b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_windows_hotspot_8u312b07.msi ;     Write-Host ('Verifying sha256 (97bfd53103e4bb8ae317c52e959e2532230d23f17af741a836490884c759b285) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '97bfd53103e4bb8ae317c52e959e2532230d23f17af741a836490884c759b285') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 26 Jan 2022 19:06:05 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0e02c12b1310e6c76c29fcd6f81905400fdb6a01caac9dc825939ad004baffef`  
		Size: 955.8 MB (955800778 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2e1f45a873642f0aab3474828d75469362741244e7c714068ac1afe056102cd6`  
		Last Modified: Thu, 20 Jan 2022 00:40:19 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc6c535d2d732c08e0c37fc29ef3fbb3e87565fb1c587ce7bf677fdd31ec1aa`  
		Last Modified: Wed, 26 Jan 2022 19:47:40 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73900f27c6d7d361de04ac8b9968b630664943a8a0bd52a09522cf5de00e77e9`  
		Last Modified: Wed, 26 Jan 2022 19:56:12 GMT  
		Size: 70.8 MB (70836165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1184b737416671eed888643ccdb01d00be78969be3b2951aeca3aab80387e5`  
		Last Modified: Wed, 26 Jan 2022 19:56:03 GMT  
		Size: 532.9 KB (532872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
