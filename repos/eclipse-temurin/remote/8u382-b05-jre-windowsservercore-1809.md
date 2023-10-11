## `eclipse-temurin:8u382-b05-jre-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:558f46032b749e30c54fa810c1a0db7d11e31e38811378c82416785f0143cb43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:8u382-b05-jre-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:f1756d9108bfda340f093b2ea2a6a9453478a872d134692fa4207d1fa96f0b91
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2104160656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2268a0d619ef08b7e2cf0d945ae58e48ec81913b91b336346c136b308c29258`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 01:36:38 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 11 Oct 2023 01:42:56 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_windows_hotspot_8u382b05.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_windows_hotspot_8u382b05.msi ;     Write-Host ('Verifying sha256 (e165227737bcc4d5c8c311cb36f8da148c552316d902f86d63c348b8ed0ca427) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e165227737bcc4d5c8c311cb36f8da148c552316d902f86d63c348b8ed0ca427') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 Oct 2023 01:44:02 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:a8471cb6f8e42a652526c77cc5029c208a54f73a0fcdff8ef4cd393e645d5dd1`  
		Last Modified: Wed, 11 Oct 2023 07:19:51 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc77e6f268346d0e9f94f81551fd854c314d10ab3f7c8f10ad4b0b73119253b`  
		Last Modified: Wed, 11 Oct 2023 07:21:05 GMT  
		Size: 72.3 MB (72268050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0120a9ff0ca8bf260b2d62d98b7c53fadac9a2ffcce191c22f2c3b065808566a`  
		Last Modified: Wed, 11 Oct 2023 07:20:57 GMT  
		Size: 299.5 KB (299510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
