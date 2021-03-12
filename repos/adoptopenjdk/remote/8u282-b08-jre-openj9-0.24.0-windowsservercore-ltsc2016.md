## `adoptopenjdk:8u282-b08-jre-openj9-0.24.0-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:20af731714fd95ca37ed2e115c8c59b97713254ca2bb16e983fe1c5b7ff6ee9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `adoptopenjdk:8u282-b08-jre-openj9-0.24.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull adoptopenjdk@sha256:e8caeacf1f0c7cbc8cae7d511e2adafd0ab1c8dce2261a5c9307a82d55ccde9d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5895617755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9990aac038199f003abfa3555777568a3ba1769650b0a5ffd3db145fc5fcd5f2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 19:53:14 GMT
ENV JAVA_VERSION=jdk8u282-b08_openj9-0.24.0
# Wed, 10 Mar 2021 19:58:44 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08_openj9-0.24.0/OpenJDK8U-jre_x64_windows_openj9_8u282b08_openj9-0.24.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08_openj9-0.24.0/OpenJDK8U-jre_x64_windows_openj9_8u282b08_openj9-0.24.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (cb1ba5f2d086ac3fb6a875ac7749837c1b0a7493d988d0b2360a0f2b392255c3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'cb1ba5f2d086ac3fb6a875ac7749837c1b0a7493d988d0b2360a0f2b392255c3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Mar 2021 19:58:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
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
	-	`sha256:23dd0034f74232dcee26f3db6305ac556dc28a7c9a402d9eeef00b54df49fb5e`  
		Last Modified: Wed, 10 Mar 2021 20:57:58 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651fbe0b7bd4f77be7ec3dc9d884f8eb97bbce29b41cfb857fcf7061b6881fc7`  
		Last Modified: Wed, 10 Mar 2021 21:04:37 GMT  
		Size: 98.7 MB (98702857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b8e42f953e9ad5676ce37242c8a011d901557e88b44c48f3347820ea2710cb`  
		Last Modified: Wed, 10 Mar 2021 21:02:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
