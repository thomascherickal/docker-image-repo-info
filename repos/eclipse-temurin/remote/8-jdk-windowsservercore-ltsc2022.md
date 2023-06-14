## `eclipse-temurin:8-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:4f49fbf9e405e37e9248a1bb2e4ba19e81952b3e2e1dd47fc5b819496fa366e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:8-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:a65d9db7f0b3e927b5a1eb060a9c4ea11aaa37d00cbf686443552d20951d82d6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1579953283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1951fb12e2fca67a5a717ed5953b3deb9beea012625ddd847cafcebb1b12c4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 17:38:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 17:38:15 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 14 Jun 2023 17:39:17 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_x64_windows_hotspot_8u372b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_x64_windows_hotspot_8u372b07.msi ;     Write-Host ('Verifying sha256 (e75a4e4a70d0fb5c0f1ca4855cb2a7f3c9ccb3d5dea5af0f45d4608a563c45b8) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e75a4e4a70d0fb5c0f1ca4855cb2a7f3c9ccb3d5dea5af0f45d4608a563c45b8') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jun 2023 17:39:48 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:34b6efc30cbc3e94b7941dacdd32d2e298ed2af399b995e08261463458618267`  
		Last Modified: Wed, 14 Jun 2023 18:18:14 GMT  
		Size: 191.1 MB (191066440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d064d3905813fd0e548e358f562192ebcec736d6b33b729da50faa8f2f04d926`  
		Last Modified: Wed, 14 Jun 2023 18:17:55 GMT  
		Size: 285.4 KB (285417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
