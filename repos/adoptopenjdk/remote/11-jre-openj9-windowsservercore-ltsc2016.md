## `adoptopenjdk:11-jre-openj9-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:999761ad005f9b9bc5a4cb79e9b946bc32c0c27e8442834ca1fbb62895bcc9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `adoptopenjdk:11-jre-openj9-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull adoptopenjdk@sha256:fe38d034be447994dadf474526b4f5b35024d81799106e1a7decf67686b95a03
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5878206848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15b5359c2e8a20822ac5f123c1ee0750325257e778bf492fa5a86d780382db64`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 20:00:51 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Wed, 10 Mar 2021 20:06:55 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_windows_openj9_11.0.10_9_openj9-0.24.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jre_x64_windows_openj9_11.0.10_9_openj9-0.24.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (66bf50f000c1803a66ccd00ccb24dbfd18a69a14731e6eb8be48f9813a6cd841) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '66bf50f000c1803a66ccd00ccb24dbfd18a69a14731e6eb8be48f9813a6cd841') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Mar 2021 20:06:56 GMT
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
	-	`sha256:0e554db5cb7f00211aed8f604e37fdf03e6af6dde3c52547009107c8821d69aa`  
		Last Modified: Wed, 10 Mar 2021 21:05:41 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5740e617ab49424c5e589883055a6d8f9ec9dc16bd7cb805f070d9d42c66ba1`  
		Last Modified: Wed, 10 Mar 2021 21:13:39 GMT  
		Size: 81.3 MB (81291856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a22985daf5b0e8869f548601c2109c79dc709afab3301fbd9a9f99eb114cc48`  
		Last Modified: Wed, 10 Mar 2021 21:13:26 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
