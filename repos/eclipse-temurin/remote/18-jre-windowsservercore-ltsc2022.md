## `eclipse-temurin:18-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:0f49ee7fce4311bf734d6e9b62a48e387b22e97e53fb75e6a77ca356b0b322fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `eclipse-temurin:18-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull eclipse-temurin@sha256:bd10400e34eb4780f141ebf2cac54c1f18a8529d14b8a7247f0f714a184bf129
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2375159558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:070e56735137b29610d4804d9f34bc136e7ecaaad8e5710c8e3e952ebe262dcb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jul 2022 15:13:23 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 13 Jul 2022 15:18:58 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_windows_hotspot_18.0.1_10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_windows_hotspot_18.0.1_10.msi ;     Write-Host ('Verifying sha256 (75a0749dfdec3f7238b0ba2572ff9b2f7debbb56710531b960d60769b1b070f5) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '75a0749dfdec3f7238b0ba2572ff9b2f7debbb56710531b960d60769b1b070f5') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-18' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Jul 2022 15:19:17 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
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
	-	`sha256:63862ff75bca4bbc059455c31a0e9f994c3e3664a4a77253a6e4302be95a66ad`  
		Last Modified: Wed, 20 Jul 2022 12:50:57 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb97b675d22834e99e51519990dc2bb915aea03a20ab5f450ac245ea75f33c`  
		Last Modified: Wed, 20 Jul 2022 12:53:18 GMT  
		Size: 74.4 MB (74353846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c7924ec680180a495744504f68d21f96bef8d1b866c88d7552046369b2a712`  
		Last Modified: Wed, 20 Jul 2022 12:53:06 GMT  
		Size: 571.3 KB (571288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
