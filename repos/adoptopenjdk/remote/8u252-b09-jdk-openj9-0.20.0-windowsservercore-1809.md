## `adoptopenjdk:8u252-b09-jdk-openj9-0.20.0-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:9eb7c5fd7f6394eae2f2f98030d91762937b1464ef3c00c4d8e19cfdc16e33fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `adoptopenjdk:8u252-b09-jdk-openj9-0.20.0-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull adoptopenjdk@sha256:e75012a2de0da5ac5f90fcd2211f0c00bfdbdc4a489367e456f9785387a1fa74
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2490071751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4212459d1e137274e08f6dd7ae74c6015b4d6e8e5900985a56abe5a1f36af2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Apr 2020 17:39:23 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 20 Apr 2020 17:41:21 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jdk_x64_windows_openj9_8u252b09_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jdk_x64_windows_openj9_8u252b09_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (5e41cb4f33b4a605f87275e4830514db20dad053cb7b5dd52bd73143abc2c7d3) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '5e41cb4f33b4a605f87275e4830514db20dad053cb7b5dd52bd73143abc2c7d3') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Mon, 20 Apr 2020 17:41:23 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
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
	-	`sha256:c9e84764eb3971bda1b806fe366008f8c4f3379bf29022d305f2e2e68bb70092`  
		Last Modified: Mon, 20 Apr 2020 18:10:45 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a5791170b1e85531107784ce1f9b09f91c4b603650a3ec1551cf648d18f9c4`  
		Last Modified: Mon, 20 Apr 2020 18:15:01 GMT  
		Size: 219.4 MB (219361088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c4883e742cbaa232b75ed56439cfddb74b27e1ed994b3c790a12537f9c4f0f`  
		Last Modified: Mon, 20 Apr 2020 18:10:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
