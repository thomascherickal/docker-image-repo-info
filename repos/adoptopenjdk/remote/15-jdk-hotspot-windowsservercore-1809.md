## `adoptopenjdk:15-jdk-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:8db3d52fbf93da3af0044d30296fe080a4de2d7799fe1a10fa44534a99e683f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `adoptopenjdk:15-jdk-hotspot-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull adoptopenjdk@sha256:baed14a99c019e4ce8130a8ff8d18024c436523d2cfd330c42cd0faf4dc2ca3e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2813471263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49aa022bb13710831e7bb1030cdda216a96490a6fecb45e068017e974cc6cbd7`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 22:15:35 GMT
ENV JAVA_VERSION=jdk-15.0.1+9
# Wed, 13 Jan 2021 22:18:10 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_windows_hotspot_15.0.1_9.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_windows_hotspot_15.0.1_9.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (7254fbe32e77a6cb8c6e36fd1da8ee0744fb323addb0bfda4c32a4d6cf9d22ce) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '7254fbe32e77a6cb8c6e36fd1da8ee0744fb323addb0bfda4c32a4d6cf9d22ce') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Jan 2021 22:18:11 GMT
CMD ["jshell"]
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
	-	`sha256:9cec778ebc246eda48b3a5b35a72ea65188a248e5ead895ed44e2a5c7ea680bd`  
		Last Modified: Wed, 13 Jan 2021 23:25:48 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39007f8248f19edcbbc9e232efbf4330769fdf59c32e37db9e5d1aa8f97ab098`  
		Last Modified: Wed, 13 Jan 2021 23:26:20 GMT  
		Size: 377.7 MB (377695741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14b0a6b2ae0a28454c85b04e217f5adced81c56c13bd4ae5bcb9ce06146bfe5`  
		Last Modified: Wed, 13 Jan 2021 23:25:47 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
