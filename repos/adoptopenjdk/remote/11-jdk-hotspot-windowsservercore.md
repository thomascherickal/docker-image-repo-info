## `adoptopenjdk:11-jdk-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:5f227a22e49ed51a6b808186423cfe10f117579d5d600c62e2532d914d58797c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64
	-	windows version 10.0.17763.1518; amd64

### `adoptopenjdk:11-jdk-hotspot-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull adoptopenjdk@sha256:1aba3d616303676bed8231ae97c95bba2b09e1c0f84df98a7514ca30d58a15eb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6111647400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61529ae96fc621eac7d944b42dba8aefc5e4564699b21a1669bdbe7653f7e75c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 19:07:35 GMT
ENV JAVA_VERSION=jdk-11.0.8+10
# Wed, 14 Oct 2020 19:10:50 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jdk_x64_windows_hotspot_11.0.8_10.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jdk_x64_windows_hotspot_11.0.8_10.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (148b487e0dde39ec5c0f32aa2397c17968b6cf6818822cea2b2394dfd0157396) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '148b487e0dde39ec5c0f32aa2397c17968b6cf6818822cea2b2394dfd0157396') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Oct 2020 19:10:51 GMT
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
	-	`sha256:290bd18aeab5461e409977bb4b19985b7197ff7cb0aa53d7ec0986a68f1a2e8b`  
		Last Modified: Wed, 14 Oct 2020 20:23:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb80acb064a8b5fbaf212fcab2f8177da4a1e92216fd8f9a85f298d93fadba66`  
		Last Modified: Wed, 14 Oct 2020 20:23:55 GMT  
		Size: 370.3 MB (370292310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24e9a3d152ef20080f41e200a6a5b9567fdd47251409a62afd27b4abbb62917`  
		Last Modified: Wed, 14 Oct 2020 20:23:24 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jdk-hotspot-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:78a473c0eabc01dfd8749aa5656fb6c238c14bb64ce157b47d7ebd7ff50040cb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2743755633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70141f0522bee0e0e6e90af642293bbe9631b13219133e93f9a65d2f572ffdf0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 19:11:02 GMT
ENV JAVA_VERSION=jdk-11.0.8+10
# Wed, 14 Oct 2020 19:13:33 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jdk_x64_windows_hotspot_11.0.8_10.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jdk_x64_windows_hotspot_11.0.8_10.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (148b487e0dde39ec5c0f32aa2397c17968b6cf6818822cea2b2394dfd0157396) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '148b487e0dde39ec5c0f32aa2397c17968b6cf6818822cea2b2394dfd0157396') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Oct 2020 19:13:34 GMT
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
	-	`sha256:4e42d4e7fec56a740b15bd9e6d08d86f73bc978926b55f9b5455d9c475fe9c94`  
		Last Modified: Wed, 14 Oct 2020 20:24:21 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbd3e27594937e7448eccdd8e2531a349f0a420ddc43e1d582c9322086718c8`  
		Last Modified: Wed, 14 Oct 2020 20:24:53 GMT  
		Size: 369.7 MB (369662059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8c11215f4b2deb55ff26a0ae1043fac8ac75da0a6958557695d6f95ba4f65c`  
		Last Modified: Wed, 14 Oct 2020 20:24:22 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
