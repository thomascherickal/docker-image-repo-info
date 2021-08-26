## `eclipse-temurin:11-jdk-windowsservercore-ltsc2016`

```console
$ docker pull eclipse-temurin@sha256:325334af57ab840b01756256f131f9dc5b557875376677151a882279f80a29e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `eclipse-temurin:11-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull eclipse-temurin@sha256:5c97b320244c46a3e04e52396f14cefdb2a05db6e476dc7831b9e01a0f637e11
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6636782880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47220838e8776c749b810627235949939fad576c01bba7b745a938b52f1fca20`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 16:42:31 GMT
ENV JAVA_VERSION=jdk-11.0.12+7
# Wed, 25 Aug 2021 16:44:04 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_windows_hotspot_11.0.12_7.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_windows_hotspot_11.0.12_7.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (80546d8a36ad0cdf69305f72f42465093b9d0388f45819b05cc640ecd1310b32) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '80546d8a36ad0cdf69305f72f42465093b9d0388f45819b05cc640ecd1310b32') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 25 Aug 2021 16:45:09 GMT
RUN Write-Host 'Verifying install ...';     Write-Host '  javac --version'; javac --version;     Write-Host '  java --version'; java --version;         Write-Host 'Complete.'
# Wed, 25 Aug 2021 16:45:10 GMT
CMD ["jshell"]
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
	-	`sha256:547314be8bafa779786b4aa68d694336bf0012275d8a56106dad8707e8ad8451`  
		Last Modified: Wed, 25 Aug 2021 23:31:43 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fb1264aaee7c67079ec62886dbe874374193bb2b2b41ed7a00d16cfdf80487`  
		Last Modified: Wed, 25 Aug 2021 23:32:12 GMT  
		Size: 365.5 MB (365499829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9d96156b18b9704f0738f687fb277fe4a846dc03a03c87ff1fd64140bbcd89`  
		Last Modified: Wed, 25 Aug 2021 23:31:43 GMT  
		Size: 312.9 KB (312899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd708cb92888ea8a599a8df23f28a589880ac6d1edd87e7cf2c86c5478026f2f`  
		Last Modified: Wed, 25 Aug 2021 23:31:43 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
