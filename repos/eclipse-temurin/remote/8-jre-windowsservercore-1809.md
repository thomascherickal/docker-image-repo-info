## `eclipse-temurin:8-jre-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:90ddbadc1b0ada8aae9d4b0090d38056f6a3ef632e8c9a94bfb822f54d9707ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:8-jre-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:5a8abf41b498cd2b6dd02b8bb23663ef6041b16aeeb5a1bc0a220f3430e5133d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784293577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c16fc52647b3d89540565a15aa7b0e2ad9672ff288bdce174f50835cbcb501b`
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
# Wed, 26 Jan 2022 19:07:43 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_windows_hotspot_8u312b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_windows_hotspot_8u312b07.msi ;     Write-Host ('Verifying sha256 (97bfd53103e4bb8ae317c52e959e2532230d23f17af741a836490884c759b285) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '97bfd53103e4bb8ae317c52e959e2532230d23f17af741a836490884c759b285') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 26 Jan 2022 19:08:50 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:e437e56dbef02b6f6eb939baf30ab4cce5a5479cf9e14f65496df00e3b041f9b`  
		Last Modified: Wed, 26 Jan 2022 19:56:32 GMT  
		Size: 70.6 MB (70632040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3d765e16df21cef10e769cb624cdeb8d6b35d30df1bc3fa958d6ed1f3be3e9`  
		Last Modified: Wed, 26 Jan 2022 19:56:23 GMT  
		Size: 337.2 KB (337203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
