## `adoptopenjdk:8u265-b01-jdk-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:4fbe84c6577ae98e03c1b29326e794f2920d0e5f0b053bd9c48d9535c0321355
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `adoptopenjdk:8u265-b01-jdk-hotspot-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:3b3bf6e54befaac6d06b53f0d0bc9d336f97abbbd9df448d0fe5a303af8f8c59
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2575119806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfa053bc0cb6c137abc7051afb61250f68da4f8e4360beeb2c005deb42b6f557`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 00:14:27 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Sat, 17 Oct 2020 00:46:41 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u265b01.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u265b01.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (3749bfd8dcc4ce3877a5b593f7df8fe05d7294435b62a919be35a003c559e033) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '3749bfd8dcc4ce3877a5b593f7df8fe05d7294435b62a919be35a003c559e033') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb5709d63eb8822ab0607f9e7bf13adeb340973ff7631cead2c9b3cb2524423`  
		Last Modified: Sat, 17 Oct 2020 01:51:29 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55b94f81701ee273c59679f901abc7909f3dea14b0e044ef297e8e611cc91c4`  
		Last Modified: Sat, 17 Oct 2020 01:55:00 GMT  
		Size: 201.0 MB (201027397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8u265-b01-jdk-hotspot-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull adoptopenjdk@sha256:ba860ca945fb7a40176cb8d0e60ed5cf7bde6757bf05309350b3b65beeef02bc
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5943014401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa274d9ecb1740ca440c15a187637df2ffe5d253fe876de596689de115421f94`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 00:47:00 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Sat, 17 Oct 2020 00:49:42 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u265b01.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_windows_hotspot_8u265b01.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (3749bfd8dcc4ce3877a5b593f7df8fe05d7294435b62a919be35a003c559e033) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '3749bfd8dcc4ce3877a5b593f7df8fe05d7294435b62a919be35a003c559e033') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:8dfe3a986471af1d9b13bc99e9a0aed2b6e497bc3dd555f0e9251dae293843a0`  
		Last Modified: Sat, 17 Oct 2020 01:55:15 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721ef409d4ab92812fd46e22dea7b8eba0aa0a4bccafde5c552a5211b3968d9d`  
		Last Modified: Sat, 17 Oct 2020 01:59:00 GMT  
		Size: 201.7 MB (201660396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
