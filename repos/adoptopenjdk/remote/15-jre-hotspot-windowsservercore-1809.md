## `adoptopenjdk:15-jre-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:697540eec22a5eb1846689650ee2af6546b1c9398c1dbecd716eed62cc217c36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `adoptopenjdk:15-jre-hotspot-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:2c23536bd9acd126e7e9c4bea2c4e6ca1f4dea56e759daca2cff6ee638f025b0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2474485813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9a5f758a75ba4ad5b2402428b3a43b22607967b93ed7d93b3a75820cb1bcc4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Sat, 17 Oct 2020 01:12:19 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_x64_windows_hotspot_15_36.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36/OpenJDK15U-jre_x64_windows_hotspot_15_36.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (d14250fb3ed06d6421c6b2e04ae266b436138213eea2fe4ddc3640df8064d9bc) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'd14250fb3ed06d6421c6b2e04ae266b436138213eea2fe4ddc3640df8064d9bc') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:636ec7c93ecd0fc88e26e6f545a6e55975f771b2fe3a22ca11a9963cdb352f12`  
		Last Modified: Sat, 17 Oct 2020 02:12:22 GMT  
		Size: 100.4 MB (100393386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
