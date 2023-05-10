## `eclipse-temurin:17-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:065ce4097ecd6281316c7da349d4174e7728abc80ec96f94a44512bfcc8dc29d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `eclipse-temurin:17-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull eclipse-temurin@sha256:800573e5feed8cb0e0083dd05b8bfc3af1af14d67976a127612e0bd9ba4cf1be
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2428644302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aa1bf757a257b89500b4f3b3777d2a18b281031aee5bbbf0eba4c8de3a42c4a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 00:56:12 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 10 May 2023 00:57:45 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_windows_hotspot_17.0.7_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_windows_hotspot_17.0.7_7.msi ;     Write-Host ('Verifying sha256 (a295dff1fd9af8341f9483202a0a96fab191438c1417c32d1f5d9ceff5927a1b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'a295dff1fd9af8341f9483202a0a96fab191438c1417c32d1f5d9ceff5927a1b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 May 2023 00:58:48 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 10 May 2023 00:58:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bf9f3ebe393d2e2543e216f5733b36e859ba5137fea21f539fd320f14abbbf`  
		Last Modified: Wed, 10 May 2023 06:59:28 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319a9034f3f31e63acbbee9a791029a086c3ffa76fd715bc036790a26c95ad3a`  
		Last Modified: Wed, 10 May 2023 06:59:52 GMT  
		Size: 352.8 MB (352781659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b40dc5ea11a828e0e0df5fa6efab2d7c007614a1622e516ad1aae493b0bc77`  
		Last Modified: Wed, 10 May 2023 06:59:29 GMT  
		Size: 3.8 MB (3823359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a947ce5a60cbf94c5fd3404723fa43441865e8cb916a18c9822924af4c27b9a9`  
		Last Modified: Wed, 10 May 2023 06:59:28 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
