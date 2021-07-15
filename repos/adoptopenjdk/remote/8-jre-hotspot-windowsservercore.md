## `adoptopenjdk:8-jre-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:2762b4643fd8a62dd367e2949f31ca940722ba2db8bbecb39d63545539442a9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `adoptopenjdk:8-jre-hotspot-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull adoptopenjdk@sha256:e4cea736768c4f687e7549a732325549eb425fae9efb20e2ca27ac8dc2ea79de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2760178247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f243d74653f674c7370b79af5854eeaaa375bbc688d10411e808e7f0fd9a742`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:25:58 GMT
ENV JAVA_VERSION=jdk8u292-b10
# Wed, 14 Jul 2021 15:31:08 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_windows_hotspot_8u292b10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_windows_hotspot_8u292b10.msi ;     Write-Host ('Verifying sha256 (4365ea6d753ce61ce809fcd94e6cda1723673b3a79b4ca71a01599eb0aecef0a) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '4365ea6d753ce61ce809fcd94e6cda1723673b3a79b4ca71a01599eb0aecef0a') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9fd60d95dfab7c8e8aff71c9567b573b9ca71ce16bdaf3282be85dca3ce71a`  
		Last Modified: Wed, 14 Jul 2021 16:37:44 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534fa2c4c5e284314ff96f641c4e3055ecf0f6994cdf25d550ecdd26338959c4`  
		Last Modified: Wed, 14 Jul 2021 16:43:35 GMT  
		Size: 74.7 MB (74728621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-hotspot-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull adoptopenjdk@sha256:7436cb5e26eb6813f1dc753b61c1957363c8349c200ffdc39cdb3c6f80549e82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6344286704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b10e341695c61f692d11ec8fa1a0eb8597aa9e7acc0b5c1c9f9c9e3b09fb3f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:27:40 GMT
ENV JAVA_VERSION=jdk8u292-b10
# Wed, 14 Jul 2021 15:33:03 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_windows_hotspot_8u292b10.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_windows_hotspot_8u292b10.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (4365ea6d753ce61ce809fcd94e6cda1723673b3a79b4ca71a01599eb0aecef0a) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '4365ea6d753ce61ce809fcd94e6cda1723673b3a79b4ca71a01599eb0aecef0a') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac0de4a2433923fda3f62862fc6e75acc7b69f6acf6714da22f1149cbfcf580`  
		Last Modified: Wed, 14 Jul 2021 16:38:19 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9495ebfb67d9d73004af77035c3a51efcae2be623a12c2b393398926a0893be9`  
		Last Modified: Wed, 14 Jul 2021 16:43:59 GMT  
		Size: 74.7 MB (74651919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
