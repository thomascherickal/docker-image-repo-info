## `eclipse-temurin:8u372-b07-jre-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:79e6ea2107d028519aa15130801bb237b3f4737b2fdb6ea063f6b6b2a61d6a78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:8u372-b07-jre-windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:284e5ee1bfddaf703dbb9019ab201e2eb3d3c74dc180f0c7be237171cb4e7461
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1460922683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba358f9e316dfb8882ca7ccd2f363f4636002646e0dde7bf51a96c07abcb5dd7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 17:38:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 17:38:15 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 14 Jun 2023 17:43:04 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_windows_hotspot_8u372b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_windows_hotspot_8u372b07.msi ;     Write-Host ('Verifying sha256 (34af6f80b9ad0351ce668a5e8968cfe9b83ee84776365320697aabe8a6d22e09) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '34af6f80b9ad0351ce668a5e8968cfe9b83ee84776365320697aabe8a6d22e09') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jun 2023 17:43:29 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972ddd233121a2afd2cf1a3eaec49d595cfe6b3ebe19ef3dd492d99784c370f`  
		Last Modified: Wed, 14 Jun 2023 18:17:55 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca63bb96f994eeeedb68d3d926ded63adca2cee41c0ef7c7b57330416b498de`  
		Last Modified: Wed, 14 Jun 2023 18:17:55 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b8156aae0419754e33ec3c933a8dc167d27a268ad94a6acb33196ead9110dd`  
		Last Modified: Wed, 14 Jun 2023 18:27:26 GMT  
		Size: 72.0 MB (72043098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ccd482c7b9e23cbfe9ab5163c00893a69de9eb5972b7f8c6589a978feeb44d`  
		Last Modified: Wed, 14 Jun 2023 18:27:18 GMT  
		Size: 278.2 KB (278159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u372-b07-jre-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:4f8974adf62d27caf0b387bfdb80460ce66137ce7f9f7c783ae0092d4b1f196d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1722974733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfc5c88393e8f2124033072d1455616ee571192df269e28e4a2aecc2c5d69255`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 17:39:58 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 14 Jun 2023 17:44:22 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_windows_hotspot_8u372b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_windows_hotspot_8u372b07.msi ;     Write-Host ('Verifying sha256 (34af6f80b9ad0351ce668a5e8968cfe9b83ee84776365320697aabe8a6d22e09) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '34af6f80b9ad0351ce668a5e8968cfe9b83ee84776365320697aabe8a6d22e09') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jun 2023 17:44:50 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc96a7c364aa977e7cc257ba13d6b4431766bcfa7630d1c030b2703486484c0a`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17d6f4661aec458185d08c3f857c6bb42a0b67f42ce7f8560957eab00a237b7`  
		Last Modified: Wed, 14 Jun 2023 18:27:44 GMT  
		Size: 72.1 MB (72071421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4992ca0ae620f634f8a76830d3eed2db8876b2e1b355b1927fd31f127da9105a`  
		Last Modified: Wed, 14 Jun 2023 18:27:35 GMT  
		Size: 280.1 KB (280125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
