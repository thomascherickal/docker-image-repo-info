## `eclipse-temurin:8u332-b09-jdk-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:65fbc2211f96ca142238c0f237a6a05a152b50403523f562219a2c6522f49aa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `eclipse-temurin:8u332-b09-jdk-windowsservercore` - windows version 10.0.20348.707; amd64

```console
$ docker pull eclipse-temurin@sha256:db86e6b650a5970bd00076cf573007de3047add798a83630e4b7d44be8d469ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2427429806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a689c88acb729fd6a13a0ad198af5eacc5139d10794ec06f9cea43041d0c49f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 14:45:34 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Wed, 11 May 2022 14:46:34 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_windows_hotspot_8u332b09.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_windows_hotspot_8u332b09.msi ;     Write-Host ('Verifying sha256 (543c46b0589d71a2dc5b18c45b94c01258aecb5bcdd9f45b5898a70bed9141fa) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '543c46b0589d71a2dc5b18c45b94c01258aecb5bcdd9f45b5898a70bed9141fa') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 May 2022 14:47:02 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad40f1b2f54a0b6277a722d0341f8258b5abade0ef4e74ec3f648c56f9f639d7`  
		Last Modified: Wed, 18 May 2022 12:43:45 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14dae3b97d91004bef699d5be707b5f86d59086658699c20323fff293e93d28`  
		Last Modified: Wed, 18 May 2022 12:44:06 GMT  
		Size: 189.3 MB (189338537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b065e0fc9dd8e8cc39c9718184cb65fdad72b62daad8f6f8334c21dbf00c1f2`  
		Last Modified: Wed, 18 May 2022 12:43:46 GMT  
		Size: 553.2 KB (553205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u332-b09-jdk-windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull eclipse-temurin@sha256:bcde92bcae8d3db55774c5c9b678d7b32376e314d7567c03aeaba2378558b143
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2693638353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53d57645ba6eb26272b946bd21a84706f42a5bd6ebdf05b0a89683f05ef023b1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 14:47:19 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Wed, 11 May 2022 14:48:38 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_windows_hotspot_8u332b09.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_windows_hotspot_8u332b09.msi ;     Write-Host ('Verifying sha256 (543c46b0589d71a2dc5b18c45b94c01258aecb5bcdd9f45b5898a70bed9141fa) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '543c46b0589d71a2dc5b18c45b94c01258aecb5bcdd9f45b5898a70bed9141fa') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 May 2022 14:49:32 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9808750119c7a9b553512f87aba9c37502f93f8fd8d580fc9e96fa2738541a3`  
		Last Modified: Wed, 18 May 2022 12:44:22 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3684ab64d9ad8a9d9cb43d5d650f598ef737d9e65c2459c5568dd83d85fb230`  
		Last Modified: Wed, 18 May 2022 12:47:50 GMT  
		Size: 189.3 MB (189255943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08db6df850dc0abc917b4a54ce5027ada289a564028791c017447501ea02aefd`  
		Last Modified: Wed, 18 May 2022 12:44:23 GMT  
		Size: 323.7 KB (323682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
