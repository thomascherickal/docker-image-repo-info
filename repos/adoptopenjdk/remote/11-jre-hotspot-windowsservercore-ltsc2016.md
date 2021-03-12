## `adoptopenjdk:11-jre-hotspot-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:c1fdfc1822bbb05b47db82ae238604a13af443bf8a860fc7dacfab2eda2613d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `adoptopenjdk:11-jre-hotspot-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull adoptopenjdk@sha256:318dc2103fb30d0e02c373d04f7c337229268879af9fb3f77f89c6a9037efcb1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5879788670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4732ff6a901de31348896c22230765ed404dab767dce93c814b4b657988aafdd`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 19:18:19 GMT
ENV JAVA_VERSION=jdk-11.0.10+9
# Wed, 10 Mar 2021 19:31:28 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.10_9.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.10_9.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (7965969a4cb913ecea276ef5e9e3bf7f145c23bd5bbdbddb9ec21384005c44fe) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '7965969a4cb913ecea276ef5e9e3bf7f145c23bd5bbdbddb9ec21384005c44fe') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:f636df8bd7077554c6e3f64570497178fe86de606b0a6f88b777c476591c7586`  
		Last Modified: Wed, 10 Mar 2021 20:35:08 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b03e7643d3e158ad427447cf720794c699febab06c2410a7f824cb25bd3343d`  
		Last Modified: Wed, 10 Mar 2021 20:38:05 GMT  
		Size: 82.9 MB (82875114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
