## `adoptopenjdk:15_36-jdk-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:b7fc9f35e9d23684e39f6725735f2c303fa3903cfe95d7d4259a6b0d221c5f38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `adoptopenjdk:15_36-jdk-hotspot-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:f905488ad30d71ebad8474cdd798877984d2d7d5f613f339cc6a43139c0cfc67
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2751566558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd0d636a1f57433212bebbd196408f460171ded23f2e0cf33c6f072d05e47d2a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 01:04:29 GMT
ENV JAVA_VERSION=jdk-15+36
# Sat, 17 Oct 2020 01:07:07 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_x64_windows_hotspot_15_36.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_x64_windows_hotspot_15_36.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (e2ac92e686e52d8c76a831319ad721547d811d2e2e9b3a8fae47420652beb930) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e2ac92e686e52d8c76a831319ad721547d811d2e2e9b3a8fae47420652beb930') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 17 Oct 2020 01:07:08 GMT
CMD ["jshell"]
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
	-	`sha256:14b6dd39a83ed26a547d74d22f7b9c4578c03229e9c114023e02de836b3d8b95`  
		Last Modified: Sat, 17 Oct 2020 02:10:02 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a93abc92f70bebc1824fb32d04885b93670214de1c7572cac0e3f8387b38bf1`  
		Last Modified: Sat, 17 Oct 2020 02:10:34 GMT  
		Size: 377.5 MB (377472971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14432d6b4d039151cc913e9f59c8a33c877f10cdbb5e73112006528486cb2ec2`  
		Last Modified: Sat, 17 Oct 2020 02:10:02 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15_36-jdk-hotspot-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull adoptopenjdk@sha256:684a9e9c723667f14a2c70b55f437ccd0ccd7d7a22e50350a0ae9e8c31c8b62b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6119463703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e67952518f26348be5676bf0c077b54a4676abc5db58ac2b3a401afad2edbc`
-	Default Command: `["jshell"]`
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
# Sat, 17 Oct 2020 01:10:40 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_x64_windows_hotspot_15_36.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jdk_x64_windows_hotspot_15_36.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (e2ac92e686e52d8c76a831319ad721547d811d2e2e9b3a8fae47420652beb930) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e2ac92e686e52d8c76a831319ad721547d811d2e2e9b3a8fae47420652beb930') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 17 Oct 2020 01:10:41 GMT
CMD ["jshell"]
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
	-	`sha256:8a70c71706c080de5e79117f20835304d14451e6809477e315a05383c1d1b8cf`  
		Last Modified: Sat, 17 Oct 2020 02:11:46 GMT  
		Size: 378.1 MB (378108574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f60079fb323752ee41e89c665c5935b82af4e9f25745357d62cb30e415b7fa`  
		Last Modified: Sat, 17 Oct 2020 02:11:15 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
