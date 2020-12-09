## `adoptopenjdk:11-jdk-hotspot-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:270edee51a98e76adbfca42d6d0108201c06a49c24692ffa8656cad5dd860620
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `adoptopenjdk:11-jdk-hotspot-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull adoptopenjdk@sha256:c13f4832166e54f6bb0697dc667dbc54641d3925f7a9125ca1906ddd514644a5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6141921860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d010f4f7cd191d32a2a7808a126bcc6b1bef2495a1b391282f80e61c768de9e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 20:34:02 GMT
ENV JAVA_VERSION=jdk-11.0.9.1+1
# Wed, 09 Dec 2020 20:37:06 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jdk_x64_windows_hotspot_11.0.9.1_1.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jdk_x64_windows_hotspot_11.0.9.1_1.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (e949c3a7d84e2423f2557e6be3f85058e1c9dc2b5615c8fb6189831e29ee2cd9) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e949c3a7d84e2423f2557e6be3f85058e1c9dc2b5615c8fb6189831e29ee2cd9') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 20:37:07 GMT
CMD ["jshell"]
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
	-	`sha256:361a5576b37a2bd2ab2b72ba4c5bab77f5d578d373e41ecae25ebd8f0d35a740`  
		Last Modified: Wed, 09 Dec 2020 21:48:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a1a8e4aa0788ab30e2a04c9c59196818c9cdadb697ad6fde067721b921669b`  
		Last Modified: Wed, 09 Dec 2020 21:48:55 GMT  
		Size: 373.1 MB (373074377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcae531158cf4d60b690aa2c526c8a0878e20e34eef5f92edf94ed4d87ee43ac`  
		Last Modified: Wed, 09 Dec 2020 21:48:26 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
