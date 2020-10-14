## `adoptopenjdk:8u262-b10-jdk-openj9-0.21.0-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:e766dcb0dd2348e611ae9d43736c5257fc5ea54b311e908db56c7bd27110e361
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `adoptopenjdk:8u262-b10-jdk-openj9-0.21.0-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:575123ad31f45a3f7edf06a0771bc5173125ecaadf7c417af122327b5d025e29
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2599186765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ea4879d3052b2f7e5b5d2d64f6eaece600cdc040a63f6668f5c41abe87d7ebf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 19:41:36 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 14 Oct 2020 19:44:07 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jdk_x64_windows_openj9_8u262b10_openj9-0.21.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jdk_x64_windows_openj9_8u262b10_openj9-0.21.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (824f32604bee0469d9dac5208dc8a025a142d95c53d838eab753bda619d46614) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '824f32604bee0469d9dac5208dc8a025a142d95c53d838eab753bda619d46614') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Oct 2020 19:44:08 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
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
	-	`sha256:77601a38c0a562d25796ba99828ae652a540978e98de66b21c021eaefc5a3a4e`  
		Last Modified: Wed, 14 Oct 2020 20:36:54 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e583ffb8a53fee552cdedbe6a507dcab95c17b84410145db6c67f6cb87409815`  
		Last Modified: Wed, 14 Oct 2020 20:37:21 GMT  
		Size: 225.1 MB (225093171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba535c30077fcdeb1560f12407db3b357bfd53fdbc32dffcaea7f02271fe2895`  
		Last Modified: Wed, 14 Oct 2020 20:36:55 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
