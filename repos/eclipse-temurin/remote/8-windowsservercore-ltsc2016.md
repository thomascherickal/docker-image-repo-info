## `eclipse-temurin:8-windowsservercore-ltsc2016`

```console
$ docker pull eclipse-temurin@sha256:a2f711eaad9aaeac26868b485cf4574ca0020ac8dfb08678610825ed2400a112
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `eclipse-temurin:8-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull eclipse-temurin@sha256:8e08e89995f4e2fc8b60a3a1c19e1355aa7e893ca159bd7c20224ca298b11e80
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6460507134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18ee8892f9f2186f52dd45b94ad553cdb98d8b9cc2ede1a1076a0d2da4ae01be`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 16:31:40 GMT
ENV JAVA_VERSION=jdk8u302-b08
# Mon, 13 Sep 2021 18:17:56 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08.1/OpenJDK8U-jdk_x64_windows_hotspot_8u302b08.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08.1/OpenJDK8U-jdk_x64_windows_hotspot_8u302b08.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (fe3546a8e8dd7d4e929028ef3794431748caddf7fc1cf481618e8d6f8aa15427) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'fe3546a8e8dd7d4e929028ef3794431748caddf7fc1cf481618e8d6f8aa15427') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 13 Sep 2021 18:18:55 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecae292a81cea3bc39342071ba043d7cca038c27464b34391354a60b8aca7f3b`  
		Last Modified: Wed, 25 Aug 2021 23:17:36 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0a9cfaabc2adaeb83d6b1c57d95f5581e79367b8c8011d78158bacb6e08831`  
		Last Modified: Mon, 13 Sep 2021 18:41:36 GMT  
		Size: 189.2 MB (189228121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c17fa0179a6d61d44da6e801c4296dc21d30e5e591a47939539b211ee49d2`  
		Last Modified: Mon, 13 Sep 2021 18:41:22 GMT  
		Size: 310.3 KB (310273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
