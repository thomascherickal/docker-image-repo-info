## `eclipse-temurin:20-jre-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:368da3923a290dc985d75eaabb34032cec69f01c9daafef4484e141d5a1f789d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:20-jre-windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:3ee7feb49b94ba62abc505b54f84acaf6e28f1a6d300d888e56cbde84b579bfd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1467222684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a4da149baf148d923280a75bf9fd26b622f08cb56ba8442e1864c74ed3250ac`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 17:38:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 18:02:31 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 14 Jun 2023 18:07:47 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ;     Write-Host ('Verifying sha256 (2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-20' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jun 2023 18:08:13 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
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
	-	`sha256:578f3890337568f3fdd8e351d5ff3132446a5b654b4108524fc132001ea8c4e7`  
		Last Modified: Wed, 14 Jun 2023 18:33:58 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261aaba9d592dc4c13bef2d69b09e2417e32c6bf9f956d8a34c8ad03f53033ba`  
		Last Modified: Wed, 14 Jun 2023 18:36:04 GMT  
		Size: 78.4 MB (78356297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d9f60cddeaa37122f58887b53c54265681e6b66b5a5dd6cc99d1c6b154e2f4`  
		Last Modified: Wed, 14 Jun 2023 18:35:53 GMT  
		Size: 265.0 KB (264967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jre-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:09f6d44b27c8ba5aaa566557b338412578844255c947d7e99a1450070c4f1a2b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1732305852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4195dc49dc2d5b8453791806d2d3f5def7a66754f042278e2e0a08e30225520c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 18:04:14 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 14 Jun 2023 18:09:07 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ;     Write-Host ('Verifying sha256 (2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-20' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jun 2023 18:09:36 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
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
	-	`sha256:cdb0557aac9b89493c8689f461e8cedea03ba66c79081f0275ee76daf7f25267`  
		Last Modified: Wed, 14 Jun 2023 18:34:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4882ee31ac08b90f7af6b602da6b632fa039f8a8599dbd2c0bc2eb2b0aa316`  
		Last Modified: Wed, 14 Jun 2023 18:36:24 GMT  
		Size: 78.4 MB (78373405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc162e88614b1717929214c40827cdd6d3087f42a698b6d825ad768545126137`  
		Last Modified: Wed, 14 Jun 2023 18:36:14 GMT  
		Size: 3.3 MB (3309278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
