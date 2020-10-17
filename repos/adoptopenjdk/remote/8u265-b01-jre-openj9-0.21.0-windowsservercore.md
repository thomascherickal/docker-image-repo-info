## `adoptopenjdk:8u265-b01-jre-openj9-0.21.0-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:fa0db6f5b50b6dd2ad020d86d0992ce7a1c77462153c96a6911f93adf7b27bfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `adoptopenjdk:8u265-b01-jre-openj9-0.21.0-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:6ccd0713092756722243dfb87625ba8979f78ee0f8439ac1a92e5d852b1ed3e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2470824427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5db4cf5171fbbae2a2162d4b2ab7612c22f45335e98beed9952ccd6716137ec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 01:14:47 GMT
ENV JAVA_VERSION=jdk8u265-b01_openj9-0.21.0
# Sat, 17 Oct 2020 01:21:22 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01_openj9-0.21.0/OpenJDK8U-jre_x64_windows_openj9_8u265b01_openj9-0.21.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01_openj9-0.21.0/OpenJDK8U-jre_x64_windows_openj9_8u265b01_openj9-0.21.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (6685611c930761f77f9499de8c992d67859887183e72aa67f3724dc81d3e2472) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '6685611c930761f77f9499de8c992d67859887183e72aa67f3724dc81d3e2472') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 17 Oct 2020 01:21:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
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
	-	`sha256:30a365cad5063acb0810d2a413c8a49ef639941ed9d6fe08ce16b6d6530b9cbf`  
		Last Modified: Sat, 17 Oct 2020 02:13:08 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aef0f4d81bc5f320fe4dadc422dc6c153f387725eb06f070ac7bf0f2b77ee19`  
		Last Modified: Sat, 17 Oct 2020 02:14:43 GMT  
		Size: 96.7 MB (96730879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c20b76a1878767a5a3c2e4b6521e6cdb4e75a91e7933fa22b8b0772fc95b1e8`  
		Last Modified: Sat, 17 Oct 2020 02:14:20 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8u265-b01-jre-openj9-0.21.0-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull adoptopenjdk@sha256:d40d11d18b93a59ff4e9655822a01d2e3139f02b2a5e0dfb98ce6b978439509d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5838713870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceb9649f557ad7fc20df659d74bd328565656e9bbd34b39c5b484755c02f0489`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 01:16:59 GMT
ENV JAVA_VERSION=jdk8u265-b01_openj9-0.21.0
# Sat, 17 Oct 2020 01:23:41 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01_openj9-0.21.0/OpenJDK8U-jre_x64_windows_openj9_8u265b01_openj9-0.21.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01_openj9-0.21.0/OpenJDK8U-jre_x64_windows_openj9_8u265b01_openj9-0.21.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (6685611c930761f77f9499de8c992d67859887183e72aa67f3724dc81d3e2472) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '6685611c930761f77f9499de8c992d67859887183e72aa67f3724dc81d3e2472') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 17 Oct 2020 01:23:41 GMT
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
	-	`sha256:7299fb27a343ed7830c455e2eda0c6da9d7244e64abe37e425fb0152df87e3de`  
		Last Modified: Sat, 17 Oct 2020 02:13:45 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9f8ba93a5367409d5b4c198b31475f80cc5e7e181218158e215dce143e7036`  
		Last Modified: Sat, 17 Oct 2020 02:15:34 GMT  
		Size: 97.4 MB (97358780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07222b4104087a229fdf9a0ca5c079f1c8bfd47226c53d6825863ac7348187f5`  
		Last Modified: Sat, 17 Oct 2020 02:14:54 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
