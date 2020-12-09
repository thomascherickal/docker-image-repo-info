## `adoptopenjdk:8-openj9-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:c746a4135e5d9358d5ad72f55cb8a7dd9ddadb5f01a19750442a5d85c7289f23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `adoptopenjdk:8-openj9-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull adoptopenjdk@sha256:0357e5b7522334cee7b4c2950c00f64eda83293fc88599d664402381db308162
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5995108107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7be001c6af59fcb662653eeb7afe76e094035867505c7739e4e5eceaa6105226`
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
# Wed, 09 Dec 2020 21:05:31 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jdk_x64_windows_openj9_8u275b01_openj9-0.23.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jdk_x64_windows_openj9_8u275b01_openj9-0.23.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (94f90bbde3cee74fb0f7708259186d54c7fa91d0519e9c8f9b363f31ddcfbb55) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '94f90bbde3cee74fb0f7708259186d54c7fa91d0519e9c8f9b363f31ddcfbb55') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 21:05:32 GMT
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
	-	`sha256:00cfc2967808ff2ffec4b4f88c0fc79dad1181b2e2f09e8dc844303cb23bdf2f`  
		Last Modified: Wed, 09 Dec 2020 21:56:15 GMT  
		Size: 226.3 MB (226260704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a74a111b5191548333528d99968548222c05ce426a320eae972ebe80a98bd3`  
		Last Modified: Wed, 09 Dec 2020 21:55:54 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
