## `adoptopenjdk:8-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:5ead63a836004602f0aefc412f8174b3760cdd6afe7e7bce54d01f2ee6d9d1f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `adoptopenjdk:8-hotspot-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull adoptopenjdk@sha256:62b4beb7b40425958b43086ee2f883b3643a96c8ebd58739f7840f7294625582
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465410790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cad2580a12c4293c2f8531116344c084a2cf9f4d2f4688ce93d8665410bc6e3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Apr 2020 17:18:06 GMT
ENV JAVA_VERSION=jdk8u252-b09
# Mon, 20 Apr 2020 17:20:09 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_x64_windows_hotspot_8u252b09.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_x64_windows_hotspot_8u252b09.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (6a2ef1781fe99ecd05f9dd7257344a271139633f6e833e1ebad4d6e6b77c744f) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '6a2ef1781fe99ecd05f9dd7257344a271139633f6e833e1ebad4d6e6b77c744f') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b30021ad9e5abf4aa83469fa9e8f04b045954d35382336e0371f88824b481`  
		Last Modified: Mon, 20 Apr 2020 18:08:56 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f4c4e59caab25cf45c8c5cfa5eaf88ea4023c5b372b112124e6e81fd13e60b`  
		Last Modified: Mon, 20 Apr 2020 18:09:17 GMT  
		Size: 194.7 MB (194701269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
