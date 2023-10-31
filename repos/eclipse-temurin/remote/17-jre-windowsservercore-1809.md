## `eclipse-temurin:17-jre-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:eda834a3e2507ade713d35be7cf8a8e719fdef94709a28a8860eeefa005e3fe4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:17-jre-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:0602b980ebaca747f1464634323973a7c46430132007238aa41c4fc7c0d637a0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2109560975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f40f7c56d831a17e5dfc9bf2ba7ab93350bce9e29dd32cb4fdd4a05fd4cd2e3d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 30 Oct 2023 23:25:59 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:31:36 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9.1/OpenJDK17U-jre_x64_windows_hotspot_17.0.9_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9.1/OpenJDK17U-jre_x64_windows_hotspot_17.0.9_9.msi ;     Write-Host ('Verifying sha256 (06a11211b09054b3a57c51c1d90fc0a183db32ee03ea0002740a0ef89d1b3cd4) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '06a11211b09054b3a57c51c1d90fc0a183db32ee03ea0002740a0ef89d1b3cd4') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 30 Oct 2023 23:32:33 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ca572b33dd9ed62ebb25ce3227b33eaa39cee409c4b93e18bc256aeb3d05fe`  
		Last Modified: Mon, 30 Oct 2023 23:50:52 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5cb03ee894f940c345937b8a0eab78c3a2e1d19f0b2d04f1b3bc491b3d8895`  
		Last Modified: Mon, 30 Oct 2023 23:52:24 GMT  
		Size: 74.8 MB (74795228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419086c246eb0ded0e093e2495b2249e965f7bdfd8ebb043655bfb648011fc6b`  
		Last Modified: Mon, 30 Oct 2023 23:52:16 GMT  
		Size: 3.2 MB (3172545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
