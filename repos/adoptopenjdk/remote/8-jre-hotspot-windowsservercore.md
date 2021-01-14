## `adoptopenjdk:8-jre-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:cf1f30455df5d9eb4ca33e5c5b58053573ab8ae0a18df833909724e84a3d944d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64
	-	windows version 10.0.14393.4169; amd64

### `adoptopenjdk:8-jre-hotspot-windowsservercore` - windows version 10.0.17763.1697; amd64

```console
$ docker pull adoptopenjdk@sha256:1f2df49756200417341c7fb45d29d43759e902c25d3b417f507a4fb3f938e60c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2519268140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3306242c7c732a96334383599e550a617b9d0e5b21a5839a65c750d72ddb0ecc`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 21:46:40 GMT
ENV JAVA_VERSION=jdk8u275-b01
# Wed, 13 Jan 2021 21:52:33 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_windows_hotspot_8u275b01.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_windows_hotspot_8u275b01.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (f5ff0ed890dd1825ae6c5f11cec06a88404835e88e511b86200fa72913542658) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f5ff0ed890dd1825ae6c5f11cec06a88404835e88e511b86200fa72913542658') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cbc8220c7600feb238762ded22e18662735ca823bf220ebd672c19dc145d9c`  
		Last Modified: Wed, 13 Jan 2021 23:09:27 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf0d77fdbd8df6e8a61917f091d5f7be5167539eff2757e321eec8fbbd9e868`  
		Last Modified: Wed, 13 Jan 2021 23:12:20 GMT  
		Size: 83.5 MB (83493725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-hotspot-windowsservercore` - windows version 10.0.14393.4169; amd64

```console
$ docker pull adoptopenjdk@sha256:6f0b8655930bc03c656823bf1b46ea79bfc4747f9e4e2f87fdcc031b22589842
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5878124959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd3c4e66a4104fc1de3ec020455a9a0242556061f8d690d6499736126ee74fad`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 21:48:37 GMT
ENV JAVA_VERSION=jdk8u275-b01
# Wed, 13 Jan 2021 21:54:42 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_windows_hotspot_8u275b01.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01/OpenJDK8U-jre_x64_windows_hotspot_8u275b01.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (f5ff0ed890dd1825ae6c5f11cec06a88404835e88e511b86200fa72913542658) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f5ff0ed890dd1825ae6c5f11cec06a88404835e88e511b86200fa72913542658') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f1d9373dd9b86ddae237ef17aff0a9050a1899613c8a619fa20f43bee6a41e`  
		Last Modified: Wed, 13 Jan 2021 23:10:06 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e155bbb8613f7d3e1b8c35818d16fb3abf19dffd7e9bea17f7dc74d16c1649`  
		Last Modified: Wed, 13 Jan 2021 23:12:55 GMT  
		Size: 84.2 MB (84228605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
