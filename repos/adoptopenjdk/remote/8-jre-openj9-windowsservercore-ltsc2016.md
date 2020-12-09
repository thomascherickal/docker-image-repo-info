## `adoptopenjdk:8-jre-openj9-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:41390498e705909a727db62368260e2db727457a46817cbbd60d525b2d6eac35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `adoptopenjdk:8-jre-openj9-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull adoptopenjdk@sha256:7cf162d36a5b60740897d54a431ae4cd3dbb3336f50545c3d970d75c18bad4b4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5866803975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27735934a85cb2e7b04bbcfe0e77a48b0388948d68c86f3e03c89d6fb17781c0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 21:03:04 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Wed, 09 Dec 2020 21:09:13 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_windows_openj9_8u275b01_openj9-0.23.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_windows_openj9_8u275b01_openj9-0.23.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (bc23f6ee03c287b75f536ac72d217be93ee1087930e1a75112af5f54f112b735) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'bc23f6ee03c287b75f536ac72d217be93ee1087930e1a75112af5f54f112b735') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 21:09:14 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
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
	-	`sha256:610a7e54f0664a6e25b04cf71ad6ba6610dd753c23ced7ab532097ab94451f6b`  
		Last Modified: Wed, 09 Dec 2020 21:55:55 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6309f6382655509a8a8192b3a0dc15c2f1aa535fadf20122c18bb4bbc3fcb9`  
		Last Modified: Wed, 09 Dec 2020 22:00:23 GMT  
		Size: 98.0 MB (97956513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bdbb6850066c7b587ee14d07a0a1bf753a1b1f3feefa210366557caa405c8ce`  
		Last Modified: Wed, 09 Dec 2020 21:58:28 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
