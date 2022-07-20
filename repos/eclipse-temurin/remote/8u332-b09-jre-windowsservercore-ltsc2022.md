## `eclipse-temurin:8u332-b09-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:34c63a4e94753996884cb924205f99b6b60155393abec7662154c7f6f2c70ff6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `eclipse-temurin:8u332-b09-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull eclipse-temurin@sha256:eab241bb4b29d05c80aad3f8d61d50a84e98e0f4b4a5763ae540bfc0eac4f437
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2371775312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4c2a812ff86375650cae9d4af4ba6196e07ef314730bb9dff6f9cd8c9909c5e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jul 2022 14:46:46 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Wed, 13 Jul 2022 14:51:58 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_x64_windows_hotspot_8u332b09.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_x64_windows_hotspot_8u332b09.msi ;     Write-Host ('Verifying sha256 (c724d3ba94f24f6ecddc6dc7367acaa4ca5b0eda828627302b8e8589dddf66c8) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'c724d3ba94f24f6ecddc6dc7367acaa4ca5b0eda828627302b8e8589dddf66c8') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Jul 2022 14:52:16 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482d99ace36f3b624267c9dff3f3365be54291445ba6046f5a6753d18e4bbf40`  
		Last Modified: Wed, 20 Jul 2022 12:42:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b941efe9907ad98a47d5939461db2f533db79bb982be7a6ed9beaac46826b948`  
		Last Modified: Wed, 20 Jul 2022 12:43:57 GMT  
		Size: 71.0 MB (70969610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f32e652985808281de7c54127acb99b186348c42524c2563f224f83f3a1773d`  
		Last Modified: Wed, 20 Jul 2022 12:43:47 GMT  
		Size: 571.3 KB (571295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
