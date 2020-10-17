## `adoptopenjdk:15_36-jre-openj9-0.22.0-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:682d045ccd399541ff71b9135f8b2cab9f7ba9d8b5786ae95e1b8a0219d167d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `adoptopenjdk:15_36-jre-openj9-0.22.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull adoptopenjdk@sha256:3457b046fcf072830d1b821c11064f77f55dfb492ca8463838f7dbd9c726a663
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836210956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755fe756f71a8f975a563e8522d6f3fc553366178773179f682a13a91e1dc614`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 01:37:37 GMT
ENV JAVA_VERSION=jdk-15+36_openj9-0.22.0
# Sat, 17 Oct 2020 01:45:18 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jre_x64_windows_openj9_15_36_openj9-0.22.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jre_x64_windows_openj9_15_36_openj9-0.22.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (78b7f6950c5afafa99164644f8dc85cd05d653964e828b52ea1916a3e27b7e61) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '78b7f6950c5afafa99164644f8dc85cd05d653964e828b52ea1916a3e27b7e61') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 17 Oct 2020 01:45:18 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086d2ce2178c7eb1c489e3433b970bcb6bfbdb0a09a5c7a1a108e787f63973a8`  
		Last Modified: Sat, 17 Oct 2020 02:23:40 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b1cff8594940dde4c495c9e74400ece5c44715b6cfe833fcbbde5cbde90575`  
		Last Modified: Sat, 17 Oct 2020 02:25:21 GMT  
		Size: 94.9 MB (94855934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf00a098f6a632488365d5e5dec1f0785ae100fd29e3125bfe8be86ec368b23`  
		Last Modified: Sat, 17 Oct 2020 02:25:08 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
