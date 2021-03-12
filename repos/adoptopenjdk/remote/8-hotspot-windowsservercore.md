## `adoptopenjdk:8-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:c2ca8900ca7f05032d7bfcf93f20407ecdd1614d94d20bbb2a9f0f0c0b101872
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `adoptopenjdk:8-hotspot-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull adoptopenjdk@sha256:df7debeb6e2c75252128b601b6cd97b434c52a0dbb062bfdac7f0690b8f8b922
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2663595096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b88760d1bd2663e7a19c21bd2ef50d659405a4920c1e874c0865ba2bfd1604c0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 18:58:24 GMT
ENV JAVA_VERSION=jdk8u282-b08
# Wed, 10 Mar 2021 19:01:26 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_windows_hotspot_8u282b08.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_windows_hotspot_8u282b08.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (fe137353ffa9f5b02c7783737e73ddf7668a3222b02c5d91abb8b8a2e55871ff) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'fe137353ffa9f5b02c7783737e73ddf7668a3222b02c5d91abb8b8a2e55871ff') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842ee128f60e6e47d30b23fa3de6f12a1b5df1a97cf9a77f57d99770469d8148`  
		Last Modified: Wed, 10 Mar 2021 20:28:43 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd4c13ea97b5973cba0ccc840dbe6cdcc1f06df3c2b1911d9195119e81831b6`  
		Last Modified: Wed, 10 Mar 2021 20:32:38 GMT  
		Size: 202.1 MB (202057796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-hotspot-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull adoptopenjdk@sha256:9c85d3ecf10eb8906b0d3c5875d27cc595be8def0068b49a883872d67b81f8ff
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5999655114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7340aca6eefdfc54cdcc365d42a35f866ec9cb68299c3dde8f32c640be26c34a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 19:01:37 GMT
ENV JAVA_VERSION=jdk8u282-b08
# Wed, 10 Mar 2021 19:07:26 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_windows_hotspot_8u282b08.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_windows_hotspot_8u282b08.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (fe137353ffa9f5b02c7783737e73ddf7668a3222b02c5d91abb8b8a2e55871ff) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'fe137353ffa9f5b02c7783737e73ddf7668a3222b02c5d91abb8b8a2e55871ff') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218fb158683ba14cc39407eb1a93ae6e224b3ce04ea064c9344436cf349b3bfe`  
		Last Modified: Wed, 10 Mar 2021 20:32:55 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e356185478448346d71e0a8883a67f901172ffe6d012f9145305a4147d740ed`  
		Last Modified: Wed, 10 Mar 2021 20:33:15 GMT  
		Size: 202.7 MB (202741558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
