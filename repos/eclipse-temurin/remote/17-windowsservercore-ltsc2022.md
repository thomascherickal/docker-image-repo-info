## `eclipse-temurin:17-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:b2c2fb485fe6a7fa69928f3335d5d44637486ee7aa480036f9317d53597027d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `eclipse-temurin:17-windowsservercore-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull eclipse-temurin@sha256:b5292676d7001115ba81fd69858c0a7c1673416739b52d9cf528d78d67c5d3dc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2244545020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7284641984f93593220c4dd56ecee52aa8438bd2eaeb8f918f0054c50ce7b122`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Sat, 02 Dec 2023 12:42:56 GMT
RUN Install update 10.0.20348.2159
# Tue, 12 Dec 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Dec 2023 00:29:18 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Wed, 13 Dec 2023 00:30:15 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9.1/OpenJDK17U-jdk_x64_windows_hotspot_17.0.9_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.9%2B9.1/OpenJDK17U-jdk_x64_windows_hotspot_17.0.9_9.msi ;     Write-Host ('Verifying sha256 (cd7b319f6fbd7efc68a0e464c55c7f2a28d6b8be3d0bcda315a16f885c57cadb) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'cd7b319f6fbd7efc68a0e464c55c7f2a28d6b8be3d0bcda315a16f885c57cadb') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Dec 2023 00:30:37 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 13 Dec 2023 00:30:38 GMT
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
	-	`sha256:dd01b46f09bf3966bd3a00527df7b3cbb66778e3c7049ad5d755023e52aec081`  
		Last Modified: Wed, 13 Dec 2023 06:38:50 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8bce710f0a295b99aa2cd05297d34890ea59e51d9effae977cdcc5d668fb8d`  
		Last Modified: Wed, 13 Dec 2023 06:39:16 GMT  
		Size: 355.0 MB (354978396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f411462561166ed6ef8b80cd96086f7f403140455190a47ea860ab1650695dd5`  
		Last Modified: Wed, 13 Dec 2023 06:38:51 GMT  
		Size: 289.0 KB (288987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3cf5a640ae2a71f1e0b4657e99507df2496cee7b944f2ef4029db87eb0e4cb`  
		Last Modified: Wed, 13 Dec 2023 06:38:50 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
