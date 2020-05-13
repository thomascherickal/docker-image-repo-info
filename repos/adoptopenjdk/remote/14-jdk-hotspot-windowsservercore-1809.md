## `adoptopenjdk:14-jdk-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:233dc083ca5d072344549fc5904203138d23e7776252b4c08ffefdf12e8f9398
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `adoptopenjdk:14-jdk-hotspot-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull adoptopenjdk@sha256:e697f8cb1a00abc1efd1dfb9ca91aeba25242d0f5cde67ec984208d2c25163a5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2104030655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:519349af1a4db0b755b8e6ed34de0e9a5ca8453dc5f750b40c5f3d27cfa7ba36`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 12:41:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 17:04:22 GMT
ENV JAVA_VERSION=jdk-14.0.1+7.1
# Wed, 13 May 2020 17:06:48 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7.1/OpenJDK14U-jdk_x64_windows_hotspot_14.0.1_7.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7.1/OpenJDK14U-jdk_x64_windows_hotspot_14.0.1_7.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (bd116ad1fb3dbe395df50068761e159348457e79aafb19f6a78d96b258aee2f2) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'bd116ad1fb3dbe395df50068761e159348457e79aafb19f6a78d96b258aee2f2') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Wed, 13 May 2020 17:06:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:77613e754ba9d62c0acd4ef271c4ee7d3af091b8c8b310afa404560a9d281f82`  
		Last Modified: Wed, 13 May 2020 13:00:20 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09430b3fa3b258d3b5d8b30b569d7294b5e692d020988cbc6cff05cbb93d261d`  
		Last Modified: Wed, 13 May 2020 18:14:17 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9700263d4d50b8e2ccd07302ad2603f6d4b6ac9106f7046962987a0cddd06a`  
		Last Modified: Wed, 13 May 2020 18:15:46 GMT  
		Size: 385.7 MB (385694359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b611a85c8f18bfdf874847aa571dcc1c4ab16def568b5b8947cd736fbd4b83ef`  
		Last Modified: Wed, 13 May 2020 18:14:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
