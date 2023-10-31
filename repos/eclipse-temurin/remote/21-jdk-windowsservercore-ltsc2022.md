## `eclipse-temurin:21-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:7d300715c6e7b519008f1fc2908f3bdff4ec4a876ba88740d29febc636e065e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `eclipse-temurin:21-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:c1f9666ae51fc0b32908276ff25e98d364790e6e0479fabf1ad1c265309a5435
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2240448296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aeac43d17d3117e9f6248b307b4fb7ebfff0d827bd2f5c5cd891b38e5e25f16`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 30 Oct 2023 23:33:00 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Mon, 30 Oct 2023 23:33:54 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_x64_windows_hotspot_21.0.1_12.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21.0.1%2B12/OpenJDK21U-jdk_x64_windows_hotspot_21.0.1_12.msi ;     Write-Host ('Verifying sha256 (62e12510b0097bd784b14b035013a32c65e7da334220c3ddfcc90d87440d240c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '62e12510b0097bd784b14b035013a32c65e7da334220c3ddfcc90d87440d240c') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-21' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 30 Oct 2023 23:34:14 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Mon, 30 Oct 2023 23:34:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2342cad8ad6a05bce2e29d23b6ae040b453d90db04b167e1041acd26752953`  
		Last Modified: Mon, 30 Oct 2023 23:52:51 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36a8ab86e955b306c51396292118175daa2d3daff7f46a9022d4a13447e4a76`  
		Last Modified: Mon, 30 Oct 2023 23:53:18 GMT  
		Size: 380.3 MB (380301295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1e656f120b4709cdf566fae48da4bf947be30d2536abebeb698f930706f93b`  
		Last Modified: Mon, 30 Oct 2023 23:52:51 GMT  
		Size: 299.7 KB (299710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b398f48a4e68e7068e0e6f3f7cc7b1e0e8829dabbfe9cd4da9dfc5f75b3732d2`  
		Last Modified: Mon, 30 Oct 2023 23:52:51 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
