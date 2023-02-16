## `eclipse-temurin:8u362-b09-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:b966a0a34dd1fc57bfc07a751de779605d1d4d3d7ae4f91548e01b67b5ee70c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `eclipse-temurin:8u362-b09-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull eclipse-temurin@sha256:c49a1da1537c087cac7916be321bc0c2bc089c8b00a9e964fd58f680b4e13686
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1752337548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821ae552bb7b1d500b41c39d96d57fbca49b70e6363da0b46254e04deb7b06bf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 22:37:50 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Wed, 15 Feb 2023 22:48:54 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_windows_hotspot_8u362b09.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_windows_hotspot_8u362b09.msi ;     Write-Host ('Verifying sha256 (fc4b3811a2cb08b1acbb6fc752ef6b2b52375406b6618baa2901f69ba0e03b9f) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'fc4b3811a2cb08b1acbb6fc752ef6b2b52375406b6618baa2901f69ba0e03b9f') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 15 Feb 2023 22:49:25 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1173e7b370b3124eddebc4b81b4e6ae4126161cfd684a7226d918a57271d9f35`  
		Last Modified: Thu, 16 Feb 2023 07:08:24 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47834e6696c7ed1e38eab55db918160ef75dfa38f81e23b3690ae4980ca5ac21`  
		Last Modified: Thu, 16 Feb 2023 07:10:15 GMT  
		Size: 72.4 MB (72405881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9857b004ec53aed91aa82b8e641f09e811dd19babd9ea2e57dc3c63ee2c313c`  
		Last Modified: Thu, 16 Feb 2023 07:10:05 GMT  
		Size: 582.5 KB (582483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
