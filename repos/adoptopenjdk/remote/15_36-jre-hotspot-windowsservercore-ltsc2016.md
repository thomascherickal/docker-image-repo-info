## `adoptopenjdk:15_36-jre-hotspot-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:7f7f45926bc86b8e48753588adbbb274b7bdce74bf36dff35a150692bf5defe6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `adoptopenjdk:15_36-jre-hotspot-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull adoptopenjdk@sha256:88d0bcc11cb31897cdce5c2d24f8450090d0b3fa910aea721be77d7bd7265509
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5842374377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e701a32be792ae63c3e0f947f39da6445f9b45bd15770c0f52b45b3e1e53a2d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 01:07:26 GMT
ENV JAVA_VERSION=jdk-15+36
# Sat, 17 Oct 2020 01:14:41 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_x64_windows_hotspot_15_36.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_x64_windows_hotspot_15_36.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (d14250fb3ed06d6421c6b2e04ae266b436138213eea2fe4ddc3640df8064d9bc) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'd14250fb3ed06d6421c6b2e04ae266b436138213eea2fe4ddc3640df8064d9bc') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:85d9ebae6a3c407b87dcad974e7425d2e65f43587d3b21c2ab9129e020030dcf`  
		Last Modified: Sat, 17 Oct 2020 02:11:15 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0161ded81e6014c55948f1b717229dfb2673219dda672ff3b5690a8571599e6`  
		Last Modified: Sat, 17 Oct 2020 02:12:57 GMT  
		Size: 101.0 MB (101020441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
