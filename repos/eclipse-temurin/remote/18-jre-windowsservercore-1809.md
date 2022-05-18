## `eclipse-temurin:18-jre-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:a884b84b58c0047d88b7330d8d734073a1d7272ceed3ff1ab4470643f61263ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `eclipse-temurin:18-jre-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull eclipse-temurin@sha256:00ff421de66135a9447bfe159d55477dd35cfb174ea967cc48dda1fae0bf81dc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2581457787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21aa5ca8aafd44a68b48e56a4a90253693f8f9409f49d66d7d82a05f910ee91f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 15:13:55 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 11 May 2022 15:20:30 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_windows_hotspot_18.0.1_10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_windows_hotspot_18.0.1_10.msi ;     Write-Host ('Verifying sha256 (75a0749dfdec3f7238b0ba2572ff9b2f7debbb56710531b960d60769b1b070f5) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '75a0749dfdec3f7238b0ba2572ff9b2f7debbb56710531b960d60769b1b070f5') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-18' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 May 2022 15:21:16 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
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
	-	`sha256:df51ff7ba754dd03b48706b43f7937a7122050287baef6e1cb1e58c077b43d64`  
		Last Modified: Wed, 18 May 2022 13:33:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed5bf600d8b22db877737f953c6c1f3ae90b421ed3718357235f32ae4f7d407`  
		Last Modified: Wed, 18 May 2022 13:42:51 GMT  
		Size: 74.2 MB (74214648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa762347ba51fcb8a5b4f1080645f9a0908300ba4b8e4314f6779d63f63a448`  
		Last Modified: Wed, 18 May 2022 13:41:34 GMT  
		Size: 3.2 MB (3184422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
