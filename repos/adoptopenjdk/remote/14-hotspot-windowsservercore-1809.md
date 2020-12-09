## `adoptopenjdk:14-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:dfab9eb5967fc88a3f2667dc84e15a109d383b160fd4102025b835733262194c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `adoptopenjdk:14-hotspot-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull adoptopenjdk@sha256:83a8ee1acda3306d2dca43875a4c28e83599e45ad8c73b0d87e5d5997ae8c4bb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2785286979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f30bb189982bef19dd8e8d44aee3496e4cf8cad5512a2ae69e48fb6d025eb7`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 20:40:51 GMT
ENV JAVA_VERSION=jdk-14.0.2+12
# Wed, 09 Dec 2020 20:43:22 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_x64_windows_hotspot_14.0.2_12.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_x64_windows_hotspot_14.0.2_12.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (9cbd03600e58ad8d2383c15e596396fbdfbc9655ba0019f5bc74c910e4082c7c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '9cbd03600e58ad8d2383c15e596396fbdfbc9655ba0019f5bc74c910e4082c7c') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 20:43:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150f2a136b619e1045702e252253091e8dcb765b949c0248950f4b9092447138`  
		Last Modified: Wed, 09 Dec 2020 21:50:11 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5f6519d16ca69cadab9b6c1e9ba3e1864cf0821c6ffac7400b1f83428e2b0d`  
		Last Modified: Wed, 09 Dec 2020 21:50:43 GMT  
		Size: 394.4 MB (394409108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c02c91efd3ba706d9bd6ff6c1288c6a8709ab9b81492ee4b68d0b6e57b8152`  
		Last Modified: Wed, 09 Dec 2020 21:50:12 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
