## `adoptopenjdk:8-jdk-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:a13701094d8fed3331bc12ee2d9bde1fcb3fbad7900472aa64443c358d8b3003
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `adoptopenjdk:8-jdk-hotspot-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull adoptopenjdk@sha256:1eea5a9aefee46895949a189b940d52d8a0d1319c7a4d1cc73f69b597de6d642
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2592575828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db285fbc162e7027cfee333211a3e302f810bf12a78a4b67693876c4961bef8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 19:53:29 GMT
ENV JAVA_VERSION=jdk8u275-b01
# Wed, 09 Dec 2020 20:25:22 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u275b01.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u275b01.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (2384cb38ad51590dd77bd171fb7198b1851cdb41ebd7a0cab19db70a3f6d7dc7) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2384cb38ad51590dd77bd171fb7198b1851cdb41ebd7a0cab19db70a3f6d7dc7') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccca71d9f2bf0560bf4d26bb7e58af228a4bdef9c4ff0d2ecb2b9e5b4837506`  
		Last Modified: Wed, 09 Dec 2020 21:45:47 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574026b73400018a3bdb81d6ddce7e87ffa101a969fa67a71688dafcad090134`  
		Last Modified: Wed, 09 Dec 2020 21:46:05 GMT  
		Size: 201.7 MB (201699160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jdk-hotspot-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull adoptopenjdk@sha256:d3e22739d1c09ba22e500d26ad71caa005ffea7ca77c46ed707b74fdfa0ad02e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5971297150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d072a75bcd0bb586cbb81c4102cb2a22d3e8ea0d473264cbaa052443244b6c09`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 20:25:31 GMT
ENV JAVA_VERSION=jdk8u275-b01
# Wed, 09 Dec 2020 20:27:53 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u275b01.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u275b01.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (2384cb38ad51590dd77bd171fb7198b1851cdb41ebd7a0cab19db70a3f6d7dc7) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2384cb38ad51590dd77bd171fb7198b1851cdb41ebd7a0cab19db70a3f6d7dc7') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bdde72856947043d93e56d0b2ce960df27f4c8467ec38ec4a3ca814fde1e22c`  
		Last Modified: Wed, 09 Dec 2020 21:46:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a49ad86eb833c586917a9730cddf2859880063d86416b76bb7e6fd8e660b19`  
		Last Modified: Wed, 09 Dec 2020 21:46:40 GMT  
		Size: 202.5 MB (202450816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
