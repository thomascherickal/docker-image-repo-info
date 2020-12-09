## `adoptopenjdk:8-jre-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:c259c6c25f82b85370dd9481f3c9193a2370a68dc3c8c1d77495488f4e1668cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `adoptopenjdk:8-jre-hotspot-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull adoptopenjdk@sha256:c1aee2d0672c121c71ddd10aceb931ef3e77b1f6782597f94f63fc535b8a5145
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2474251525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52e701f6f3cf25122dd4aa45b758e54ba987f288651d3402d537fba3bad493ac`
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
# Wed, 09 Dec 2020 20:29:11 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_windows_hotspot_8u275b01.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_windows_hotspot_8u275b01.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (f5ff0ed890dd1825ae6c5f11cec06a88404835e88e511b86200fa72913542658) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f5ff0ed890dd1825ae6c5f11cec06a88404835e88e511b86200fa72913542658') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:ff65b27b0afe93e062ec6f7640d3c440bb7b20ebeffbbf50f48b193f73b84ade`  
		Last Modified: Wed, 09 Dec 2020 21:47:05 GMT  
		Size: 83.4 MB (83374857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-hotspot-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull adoptopenjdk@sha256:236ea8f64722e9ce19aa92740aac1507d6afbb1f1e9898117a8424643f93b6cd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5852973560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37704eb853566e1d9c61af7ef91bc87c13a729169ee143df4e41476806ef1902`
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
# Wed, 09 Dec 2020 20:31:15 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_windows_hotspot_8u275b01.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_windows_hotspot_8u275b01.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (f5ff0ed890dd1825ae6c5f11cec06a88404835e88e511b86200fa72913542658) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f5ff0ed890dd1825ae6c5f11cec06a88404835e88e511b86200fa72913542658') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:f75767b86d36919bafc394353496bae4e0a51301621408368b2d0c8ebd407b8b`  
		Last Modified: Wed, 09 Dec 2020 21:47:28 GMT  
		Size: 84.1 MB (84127226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
