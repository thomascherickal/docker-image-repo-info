## `eclipse-temurin:8u312-b07-jre-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:486f08c2321da8508c190ca212a0e3dcaa97c6cb525ff982712a1d7c5cfcdf55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.469; amd64
	-	windows version 10.0.17763.2452; amd64

### `eclipse-temurin:8u312-b07-jre-windowsservercore` - windows version 10.0.20348.469; amd64

```console
$ docker pull eclipse-temurin@sha256:978ed01e4692c38bb5be68e7c63ae17637e530d29043ea97630509f4f6feddf7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2279140908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88e276ddb87057754d4fe964ac51ca10b15a333ca4a4cb1623746ca814b6f3f1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 06 Jan 2022 03:56:33 GMT
RUN Install update ltsc2022-amd64
# Tue, 11 Jan 2022 18:59:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 21:28:50 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Tue, 11 Jan 2022 21:38:07 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_windows_hotspot_8u312b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_windows_hotspot_8u312b07.msi ;     Write-Host ('Verifying sha256 (97bfd53103e4bb8ae317c52e959e2532230d23f17af741a836490884c759b285) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '97bfd53103e4bb8ae317c52e959e2532230d23f17af741a836490884c759b285') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Tue, 11 Jan 2022 21:38:30 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b593686e27e7562a5b0696823307ffa822214cee8bd2eec1075eadad4cb9712`  
		Size: 956.0 MB (956001983 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:99e0b71ede60d3b2c5b9053bf27e47c0875590991eede49813d849cc660c7551`  
		Last Modified: Tue, 11 Jan 2022 19:32:06 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530438f2b1a82fa7955135e41d90fcb4778b5320efa44edfc8df468938f014cd`  
		Last Modified: Tue, 11 Jan 2022 22:37:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d328544dc8ba9427f59fdbefbdfd5bb914dd6a1224acd7cf3946a91502a823e9`  
		Last Modified: Tue, 11 Jan 2022 22:47:19 GMT  
		Size: 70.9 MB (70870608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed0fe1bedc6adb67e160bd42f4afdb077b920e49fd66c310d3af7ff4f4dec5a`  
		Last Modified: Tue, 11 Jan 2022 22:47:11 GMT  
		Size: 566.5 KB (566522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u312-b07-jre-windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull eclipse-temurin@sha256:466174cc662afc76127bfcf46c8cde9e51e65bc97617b91bfe323f4ade197919
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2783144836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:721c8001160bb532ef40074f0df361b542a44910bdde71dfaafc5ff4faec77f1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 05:11:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 15:31:05 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 12 Jan 2022 15:36:33 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_windows_hotspot_8u312b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_windows_hotspot_8u312b07.msi ;     Write-Host ('Verifying sha256 (97bfd53103e4bb8ae317c52e959e2532230d23f17af741a836490884c759b285) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '97bfd53103e4bb8ae317c52e959e2532230d23f17af741a836490884c759b285') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 12 Jan 2022 15:37:31 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3a70d5fd54e2005efbf590b48700ed40509210354a0d8f3f18c3b444a5325896`  
		Last Modified: Wed, 12 Jan 2022 06:20:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1440152d7fe8d63c5c9773cf2bbc39cd20d7d90bc195ba351f6795634011b`  
		Last Modified: Wed, 12 Jan 2022 16:01:37 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0516dddde406b1ed8908739c4ac9d07874f98e249bdaedc77b44e54e625499c2`  
		Last Modified: Wed, 12 Jan 2022 16:05:50 GMT  
		Size: 70.6 MB (70599803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578320c68ff382e6eac6e6759202ab6b368ba419ef1167eafafede380a3766e7`  
		Last Modified: Wed, 12 Jan 2022 16:05:42 GMT  
		Size: 311.3 KB (311333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
