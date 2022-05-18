## `eclipse-temurin:8-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:17dd6b935dfd3598949dc54f0fe351832f443552ef9fef7245cad002d3745dc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `eclipse-temurin:8-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull eclipse-temurin@sha256:084f972439b19fad8a7e630d2cacbe08a8b78b917ee350998c3fa59d11a106c1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2309013243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d26474dfde26fedbdcfa4023c86e492cbffb461a4c7fa72d263f1a6d5091a05c`
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
# Wed, 11 May 2022 14:51:42 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_x64_windows_hotspot_8u332b09.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_x64_windows_hotspot_8u332b09.msi ;     Write-Host ('Verifying sha256 (c724d3ba94f24f6ecddc6dc7367acaa4ca5b0eda828627302b8e8589dddf66c8) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'c724d3ba94f24f6ecddc6dc7367acaa4ca5b0eda828627302b8e8589dddf66c8') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 May 2022 14:52:02 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:926a3faf65360001bcc2802348324e1e8aa0a40beaf4bf3fddc6e504f8fd37b8`  
		Last Modified: Wed, 18 May 2022 12:51:22 GMT  
		Size: 70.9 MB (70922320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b07ab9b28297828aa8e0db25161f3e13a1d6932b558c5a80feb5f2a58f78f2c`  
		Last Modified: Wed, 18 May 2022 12:50:07 GMT  
		Size: 552.9 KB (552859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
