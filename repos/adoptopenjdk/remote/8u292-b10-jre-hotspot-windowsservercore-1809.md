## `adoptopenjdk:8u292-b10-jre-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:1b642d22b4cae36172b0cf4d122ead7e7ce1813c5de837150271d8aeeff04965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `adoptopenjdk:8u292-b10-jre-hotspot-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull adoptopenjdk@sha256:0d288497b62da5b3afa00c28f21a8a38b2d486e6eb31fba25e417bc34b2012dd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2553952029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdedf993836944920a5c5f49541cb7f91ae50e530691d4e92a2c0009a2bc06f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 17:37:20 GMT
ENV JAVA_VERSION=jdk8u292-b10
# Wed, 12 May 2021 17:42:15 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_windows_hotspot_8u292b10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jre_x64_windows_hotspot_8u292b10.msi ;     Write-Host ('Verifying sha256 (4365ea6d753ce61ce809fcd94e6cda1723673b3a79b4ca71a01599eb0aecef0a) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '4365ea6d753ce61ce809fcd94e6cda1723673b3a79b4ca71a01599eb0aecef0a') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4850affec9717aa76f17b1708a82a204074fe1e1288ddb43fb790c40690b7552`  
		Last Modified: Wed, 12 May 2021 18:45:59 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7359cf818a580e3c14c636c29750ef5dba32507ae68f9473f5948a265cead8`  
		Last Modified: Wed, 12 May 2021 18:57:22 GMT  
		Size: 79.5 MB (79460049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
