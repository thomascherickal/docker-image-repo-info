## `adoptopenjdk:8u292-b10-jre-openj9-0.26.0-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:8b773b57a15474edfea88a003f9c1d7b228c6f2361d2a0c0a7b1fc380c2f0cf1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `adoptopenjdk:8u292-b10-jre-openj9-0.26.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull adoptopenjdk@sha256:db72e18f74e41ef661f8b209819bf22b4627d1dbd6ea05496c5810ed5a9ca705
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.4 GB (6362162716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8141526b320ab696a899dbc0eac563c867f7c282cdfb22cf70e7e6fa460e668`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 19:23:05 GMT
ENV JAVA_VERSION=jdk8u292-b10_openj9-0.26.0
# Wed, 11 Aug 2021 19:29:12 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jre_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jre_x64_windows_openj9_8u292b10_openj9-0.26.0.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (8decae9e065946cfc9a4b7f3c0ed61cfc6fe3076cdcbbbece33ef39c9ccef6e3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8decae9e065946cfc9a4b7f3c0ed61cfc6fe3076cdcbbbece33ef39c9ccef6e3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 Aug 2021 19:29:15 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558fb52ac1a6286b9fe2620f6511643452589728c2bd11423d63b7b03d5ef250`  
		Last Modified: Wed, 11 Aug 2021 20:35:08 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a49edf30f3dfa3dcf89ba973b6d0239d05c3acbf97dc77b0c6c9d2c58025b`  
		Last Modified: Wed, 11 Aug 2021 20:40:12 GMT  
		Size: 91.2 MB (91192437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4212095ae2483bc701fe645538b03b598b38f2a93d84177dc0834a5504713a`  
		Last Modified: Wed, 11 Aug 2021 20:40:03 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
