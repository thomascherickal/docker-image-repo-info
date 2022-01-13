## `eclipse-temurin:11-jre-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:97a98ec0d183340e170a2fce06d173840b3dd6211e26185ad6eb36b9f254195a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.469; amd64
	-	windows version 10.0.17763.2452; amd64

### `eclipse-temurin:11-jre-windowsservercore` - windows version 10.0.20348.469; amd64

```console
$ docker pull eclipse-temurin@sha256:c1f80b33b106b395d114e0418590073472b9a72ad6a7c94e77430af1be062842
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2282129926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70d02d2acf88c55bccc31ce8e36b673e22d5ed794de661d4d8bc276a49180d1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 06 Jan 2022 03:56:33 GMT
RUN Install update ltsc2022-amd64
# Tue, 11 Jan 2022 18:59:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 21:44:02 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Tue, 11 Jan 2022 21:55:41 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_windows_hotspot_11.0.13_8.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_windows_hotspot_11.0.13_8.msi ;     Write-Host ('Verifying sha256 (4ca99c580144de53b2b8b023cbf755445e2f5f34239856e4ce92e3ea5a1b15b9) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '4ca99c580144de53b2b8b023cbf755445e2f5f34239856e4ce92e3ea5a1b15b9') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Tue, 11 Jan 2022 21:56:04 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
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
	-	`sha256:43165977fb6450651cbd2d709f0002c2df0e1dd90d01ccb8a64230f4501cac12`  
		Last Modified: Tue, 11 Jan 2022 22:48:22 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af4100848539b9068aaa89604f065d1d5c1a80b5072a66d4c86c90473309be9`  
		Last Modified: Tue, 11 Jan 2022 23:00:42 GMT  
		Size: 73.9 MB (73860534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1912c376de93ae7a3456ee00beacf79b06b3bad2a7b253de54dff7298cb48e7`  
		Last Modified: Tue, 11 Jan 2022 23:00:32 GMT  
		Size: 565.7 KB (565744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull eclipse-temurin@sha256:9fb23242902ea6042199c03c96da36e862b31b99aaae9b66cc4045c85a5a36f9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2786137404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a16ded612dd39a350a68d5e30333f9a243e2731257f00b3ceba9b3d066c038d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 05:11:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 15:38:14 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 12 Jan 2022 15:44:39 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_windows_hotspot_11.0.13_8.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_windows_hotspot_11.0.13_8.msi ;     Write-Host ('Verifying sha256 (4ca99c580144de53b2b8b023cbf755445e2f5f34239856e4ce92e3ea5a1b15b9) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '4ca99c580144de53b2b8b023cbf755445e2f5f34239856e4ce92e3ea5a1b15b9') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 12 Jan 2022 15:45:35 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
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
	-	`sha256:16eb147e9236ff1784d2b515ebeec87c4e063c5d89ad69df593a41b5c24292e6`  
		Last Modified: Wed, 12 Jan 2022 16:06:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19962110dd419364f5f642c6718446cce087e04bd9a28820b49aea8cfa4d7f25`  
		Last Modified: Wed, 12 Jan 2022 16:13:57 GMT  
		Size: 73.6 MB (73592615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb8de3b93895c8d6bfaac1fa7a779b525f51e412cfd3424645e2c68c6b2454d`  
		Last Modified: Wed, 12 Jan 2022 16:13:47 GMT  
		Size: 311.1 KB (311053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
