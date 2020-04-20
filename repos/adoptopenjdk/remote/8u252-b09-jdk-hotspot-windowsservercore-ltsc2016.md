## `adoptopenjdk:8u252-b09-jdk-hotspot-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:58a475f0784ac47b4b717630a81120f4a30a62b2b705e554e038ebf37dd19e43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `adoptopenjdk:8u252-b09-jdk-hotspot-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull adoptopenjdk@sha256:57221de5d23ac5c173d3351398896c14d354b6ad91d3c152bb7c471e03f44543
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5927932996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f939313e88e9696c48aec91ed87686eac99f571fc032398cf02f5a092967a82`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Apr 2020 17:15:28 GMT
ENV JAVA_VERSION=jdk8u252-b09
# Mon, 20 Apr 2020 17:17:59 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_x64_windows_hotspot_8u252b09.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_x64_windows_hotspot_8u252b09.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (6a2ef1781fe99ecd05f9dd7257344a271139633f6e833e1ebad4d6e6b77c744f) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '6a2ef1781fe99ecd05f9dd7257344a271139633f6e833e1ebad4d6e6b77c744f') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5817d04a2349b002655920bf800136b2997626291751b4ea8bac4b1ac9933e`  
		Last Modified: Mon, 20 Apr 2020 18:08:22 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0341b03ef549deb8a5b53ca5a298df330a3cba6db2573fec815f8719816fbf`  
		Last Modified: Mon, 20 Apr 2020 18:08:42 GMT  
		Size: 199.9 MB (199863145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
