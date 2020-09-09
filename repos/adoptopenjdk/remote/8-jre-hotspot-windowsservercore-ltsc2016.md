## `adoptopenjdk:8-jre-hotspot-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:dae3b955bd6a8e909d92dca35e42ddd45df9bec024c01e80024654e98b01270b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `adoptopenjdk:8-jre-hotspot-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull adoptopenjdk@sha256:c6b67bf574fe22203afacfb2157dc5edc146d6083d4317bdac32a9f48271dfa1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5822705775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96808fac9219513441b5404213b1b79b3148acf9496328b9820c8d230775c06`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 17:23:45 GMT
ENV JAVA_VERSION=jdk8u262-b10
# Wed, 09 Sep 2020 18:00:04 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jre_x64_windows_hotspot_8u262b10.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jre_x64_windows_hotspot_8u262b10.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (e85f21cddd791f1b362de285338912de60ee12d7fd27847faeee37f294f7a06b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e85f21cddd791f1b362de285338912de60ee12d7fd27847faeee37f294f7a06b') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:dfa6b3d0213a8f1eb2bcf8b89d3056f18e02dcb19b71fd1ce958125b0a126bc6`  
		Last Modified: Wed, 09 Sep 2020 19:11:52 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203f1903726b35c3fd4bae14174a6eb619dfa59c5faac92660d485e39ae92ca8`  
		Last Modified: Wed, 09 Sep 2020 19:13:13 GMT  
		Size: 83.4 MB (83448979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
