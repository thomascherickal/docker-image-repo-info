## `adoptopenjdk:8u232-b09-jdk-openj9-0.17.0-windowsservercore-1803`

```console
$ docker pull adoptopenjdk@sha256:e2b311f7bb73e49ca2c592aac2c78960edfbd81b61c6e1c29ffc074bae6798c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17134.1246; amd64

### `adoptopenjdk:8u232-b09-jdk-openj9-0.17.0-windowsservercore-1803` - windows version 10.0.17134.1246; amd64

```console
$ docker pull adoptopenjdk@sha256:877ff0fc8f4fe69d911e6cd2de5b373e6503e837cfbf0894a01fe8da56b1f56c
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2582364201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:900493f5efb4627308871f6f5d313ec9d3308f1249e4bdc3bcc3c5917676ba76`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 12 Apr 2018 09:20:54 GMT
RUN Apply image 1803-RTM-amd64
# Wed, 08 Jan 2020 15:30:02 GMT
RUN Install update 1803-amd64
# Wed, 15 Jan 2020 18:58:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 19:47:01 GMT
ENV JAVA_VERSION=jdk8u232-b09_openj9-0.17.0
# Wed, 15 Jan 2020 19:49:34 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jdk_x64_windows_openj9_8u232b09_openj9-0.17.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jdk_x64_windows_openj9_8u232b09_openj9-0.17.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (c0c64822a4b657f2ac2b2185a7113070d57380153d2e1d6c20e04aa33cb295ae) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'c0c64822a4b657f2ac2b2185a7113070d57380153d2e1d6c20e04aa33cb295ae') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Wed, 15 Jan 2020 19:49:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:d9e8b01179bfc94a5bdb1810fbd76b999aa52016001ace2d3a4c4bc7065a9601`  
		Last Modified: Tue, 18 Sep 2018 22:43:55 GMT  
		Size: 1.7 GB (1659688273 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:270ec3ad3fc7d52c0dd086b32f7751131c799e25cdcd4686cc33cbf2b607c34e`  
		Size: 699.2 MB (699246147 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4b8ccd780af5210d26057ebca3a11489d01a7a0151f175a60af96d3719ce8bc9`  
		Last Modified: Wed, 15 Jan 2020 20:45:08 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ac9d587454f0ceaa267a468ec3a6de1283d5c3bafc1076c42dba025cf3a56a`  
		Last Modified: Wed, 15 Jan 2020 21:06:58 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37651b3eac5addd5fc06e6bc9d4a1b0d71aa2c8a5f5ff08f2abed398761bfdbb`  
		Last Modified: Wed, 15 Jan 2020 21:07:43 GMT  
		Size: 223.4 MB (223426149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6913ddde7b2ba2eee4f5c6e12f755d733efeeac5f83bc775ee5fae6abe559f69`  
		Last Modified: Wed, 15 Jan 2020 21:06:58 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
