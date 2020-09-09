## `adoptopenjdk:8u262-b10-jdk-openj9-0.21.0-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:9a62bcedde5e110c57e07a93c8ae26e16ee6e15201625a3703bc56d9f76b6f9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `adoptopenjdk:8u262-b10-jdk-openj9-0.21.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull adoptopenjdk@sha256:75881243c96d79bc69045853823d3a8a12482aaad800e75087ebb3ada7b0547f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5964949308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34aa893721be0ffb3bd24e9a15d0492fbb2d121ce05bd1b72c3be04265e13185`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 18:30:49 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 09 Sep 2020 18:33:21 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jdk_x64_windows_openj9_8u262b10_openj9-0.21.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jdk_x64_windows_openj9_8u262b10_openj9-0.21.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (824f32604bee0469d9dac5208dc8a025a142d95c53d838eab753bda619d46614) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '824f32604bee0469d9dac5208dc8a025a142d95c53d838eab753bda619d46614') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Sep 2020 18:33:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2a5d2ad6dfb4a3920b8f5bb1f429da73048604381fe4d570e8093c7a289b30`  
		Last Modified: Wed, 09 Sep 2020 19:29:57 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43362159cb34aa39c755e52503cd03420a56000417a5bb322d164d2338550caa`  
		Last Modified: Wed, 09 Sep 2020 19:30:17 GMT  
		Size: 225.7 MB (225691419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205e8415224c39de64f5a72050505d3e905b2a5e438a610d627f541d495512df`  
		Last Modified: Wed, 09 Sep 2020 19:29:58 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
