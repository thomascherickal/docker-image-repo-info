## `adoptopenjdk:8u275-b01-jdk-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:7f9a199dd09432989aae4a1fe4da9990298e336bcb8ccdf465f7190b99a314fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `adoptopenjdk:8u275-b01-jdk-hotspot-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull adoptopenjdk@sha256:7563a31621b895a382e554f286525e5da40d1b94bd5b69d32c1cd98545053d28
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2637596102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cb529846c47d25cfcb149daaa1809f08d858cd4ac682fc7f0dcb2738f2ed98a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 21:46:40 GMT
ENV JAVA_VERSION=jdk8u275-b01
# Wed, 13 Jan 2021 21:48:29 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u275b01.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u275b01.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (2384cb38ad51590dd77bd171fb7198b1851cdb41ebd7a0cab19db70a3f6d7dc7) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2384cb38ad51590dd77bd171fb7198b1851cdb41ebd7a0cab19db70a3f6d7dc7') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cbc8220c7600feb238762ded22e18662735ca823bf220ebd672c19dc145d9c`  
		Last Modified: Wed, 13 Jan 2021 23:09:27 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360ee8df72cde7d2aacfc2cb6fc497a50225e5031a6fe799a3a031903e4085e1`  
		Last Modified: Wed, 13 Jan 2021 23:09:46 GMT  
		Size: 201.8 MB (201821687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8u275-b01-jdk-hotspot-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull adoptopenjdk@sha256:d58a8e440d5a75190d59e8f898bdd217444ffc7c7adca5da941c2d673ce0b312
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5996451988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc807954baae08c0e76698bedf40e170c849181a00df0e895ac168b13e23fbdd`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 21:48:37 GMT
ENV JAVA_VERSION=jdk8u275-b01
# Wed, 13 Jan 2021 21:51:06 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u275b01.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u275b01.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (2384cb38ad51590dd77bd171fb7198b1851cdb41ebd7a0cab19db70a3f6d7dc7) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2384cb38ad51590dd77bd171fb7198b1851cdb41ebd7a0cab19db70a3f6d7dc7') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f1d9373dd9b86ddae237ef17aff0a9050a1899613c8a619fa20f43bee6a41e`  
		Last Modified: Wed, 13 Jan 2021 23:10:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe64fc71ab83699145b9ee13b1c7e3090525287b9c79c4ed3f8820d2427a554`  
		Last Modified: Wed, 13 Jan 2021 23:10:26 GMT  
		Size: 202.6 MB (202555634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
