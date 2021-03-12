## `adoptopenjdk:14-openj9-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:d0a6a20ac657a3442719aaf569bb68d894e1768639248213420cf1d97ce5f1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `adoptopenjdk:14-openj9-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull adoptopenjdk@sha256:7ca8b339db0edaeadd9e480a0c65501efe835cbe721822b059db01cb9bc076bc
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6191509701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b28799f00ba78b517cb87d31524a895bbfddb0792ba4ec65205a3f11d19e60f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 20:09:16 GMT
ENV JAVA_VERSION=jdk-14.0.2+12_openj9-0.21.0
# Wed, 10 Mar 2021 20:11:50 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12_openj9-0.21.0/OpenJDK14U-jdk_x64_windows_openj9_14.0.2_12_openj9-0.21.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12_openj9-0.21.0/OpenJDK14U-jdk_x64_windows_openj9_14.0.2_12_openj9-0.21.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (2e496ce7ca02f7a380fd1902e06d55d52121bb2eee29b21b8e54ad3e2fd3466e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2e496ce7ca02f7a380fd1902e06d55d52121bb2eee29b21b8e54ad3e2fd3466e') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Mar 2021 20:11:51 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 10 Mar 2021 20:11:52 GMT
CMD ["jshell"]
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
	-	`sha256:ded9640e9c1207c5c4c7ef1d7ba688c5bf024f299741b66ee2613db379e62766`  
		Last Modified: Wed, 10 Mar 2021 21:14:47 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bf90f34657434d35c90a96f8bb83cbc923470cbb4275bfa6d3d8782f6bf241`  
		Last Modified: Wed, 10 Mar 2021 21:15:21 GMT  
		Size: 394.6 MB (394593296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a09029bead8c83d4d6783a2181e664f7cccd332ffb38ad4fb79edd226c6bbd4`  
		Last Modified: Wed, 10 Mar 2021 21:14:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14272b3eb81c0856fc5ff1acc3651e84848aa817d1f8ef510fefd6457ce831d`  
		Last Modified: Wed, 10 Mar 2021 21:14:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
