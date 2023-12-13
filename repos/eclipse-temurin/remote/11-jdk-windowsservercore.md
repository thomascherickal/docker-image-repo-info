## `eclipse-temurin:11-jdk-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:7829416b913e624c4b6a8793144b992ce13aa98655ef1e832329099dcc155346
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:11-jdk-windowsservercore` - windows version 10.0.20348.2159; amd64

```console
$ docker pull eclipse-temurin@sha256:90c27f74b8186848a30232401e889303ec17ea4a19b5064614709be189bd4a69
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258676528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148aae18f84a2c62f6477a839cbaeddf569a4deb4b2ed15ec29f08a0f8809606`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Tue, 12 Dec 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 00:19:32 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 13 Dec 2023 00:20:32 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.21_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.21_9.msi ;     Write-Host ('Verifying sha256 (ccaa09811f488cf95340e2702e8d9176058a52e89808ae6e1a1d20de39e5ce34) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'ccaa09811f488cf95340e2702e8d9176058a52e89808ae6e1a1d20de39e5ce34') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Dec 2023 00:21:00 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 13 Dec 2023 00:21:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7839fc47f6e056f9e09a214230f8b7115e69419dbc74acbbb1ad6bc0caa28862`  
		Last Modified: Tue, 12 Dec 2023 18:27:40 GMT  
		Size: 500.7 MB (500674814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d0c853ded9068434b9128a8016b3ae5e18f748f62801c7bb6e6092495300ec`  
		Last Modified: Wed, 13 Dec 2023 00:02:39 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455780d2f42600efb2a3a20116e117f6d5c0f47e123f17be7a83db9c2c69bf42`  
		Last Modified: Wed, 13 Dec 2023 06:36:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f6b6d6d254a66ea8855b57f47e10deafe76cb38119778edbeffffd44896368`  
		Last Modified: Wed, 13 Dec 2023 06:36:40 GMT  
		Size: 369.1 MB (369109896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e926117d3d6655766696b632c45d33c84c59b0d4e4fccf3b8ec01807be27f648`  
		Last Modified: Wed, 13 Dec 2023 06:36:14 GMT  
		Size: 289.0 KB (289025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e162c4f80d9186be8c007d1a3abbaacaf7230bfe887db54ca3ebb11a3ea08890`  
		Last Modified: Wed, 13 Dec 2023 06:36:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk-windowsservercore` - windows version 10.0.17763.5206; amd64

```console
$ docker pull eclipse-temurin@sha256:3bb63ca8fee16e74caaa2e358ea266a076b152b0e7480fec5a471d502080019c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2429148177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c88cd63979664f42419929b9c3e34a2b084754400a1dc8e4a1ec8b143eb5a0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Tue, 12 Dec 2023 23:38:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 00:21:15 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 13 Dec 2023 00:22:53 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.21_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.21_9.msi ;     Write-Host ('Verifying sha256 (ccaa09811f488cf95340e2702e8d9176058a52e89808ae6e1a1d20de39e5ce34) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'ccaa09811f488cf95340e2702e8d9176058a52e89808ae6e1a1d20de39e5ce34') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Dec 2023 00:23:58 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 13 Dec 2023 00:23:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767e95390edb4050b2c57e1d564c9e4722c5ae776ebfb8907a539571a2609f7c`  
		Last Modified: Wed, 13 Dec 2023 00:04:16 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22613c8f55cb8faa07b5c958077cfbefb515e8040ee3f5f8d4c23a6b9c85a5ec`  
		Last Modified: Wed, 13 Dec 2023 06:36:52 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e065aa6f33926f10e0734001109a6fd1d16f004cd82e04f83307ec384ae76d05`  
		Last Modified: Wed, 13 Dec 2023 06:37:18 GMT  
		Size: 369.1 MB (369148499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f5bf6e7572a5553920e254264b5ed338542218d5e10dd83845060e0778cd98`  
		Last Modified: Wed, 13 Dec 2023 06:36:52 GMT  
		Size: 286.7 KB (286732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4882915a066592db64632cfeaf0305c605c6951df3df0a267ca79a60657a471`  
		Last Modified: Wed, 13 Dec 2023 06:36:52 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
