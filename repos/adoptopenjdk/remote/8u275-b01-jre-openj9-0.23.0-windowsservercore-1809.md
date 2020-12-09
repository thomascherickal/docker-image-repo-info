## `adoptopenjdk:8u275-b01-jre-openj9-0.23.0-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:37241aa2caf84baf6d3d51fb6ddade4e2a70358006a98ff03ac9125d7ad325e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `adoptopenjdk:8u275-b01-jre-openj9-0.23.0-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull adoptopenjdk@sha256:4b7ae5cf05ac45a19034616bc59e6e90d738b13b85a5b870ea391cb77ca75f46
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488088402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93864f0cfa943b4af2a3a8d09d4e781d6dc77429e2e4602c82eb340aa61d3406`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 21:00:53 GMT
ENV JAVA_VERSION=jdk8u275-b01_openj9-0.23.0
# Wed, 09 Dec 2020 21:07:06 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_windows_openj9_8u275b01_openj9-0.23.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u275-b01_openj9-0.23.0/OpenJDK8U-jre_x64_windows_openj9_8u275b01_openj9-0.23.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (bc23f6ee03c287b75f536ac72d217be93ee1087930e1a75112af5f54f112b735) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'bc23f6ee03c287b75f536ac72d217be93ee1087930e1a75112af5f54f112b735') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 21:07:07 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
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
	-	`sha256:f7e512927381b14660b382af0dbe3be4d4b3ccf73d36c68934f3f0c786a5bb30`  
		Last Modified: Wed, 09 Dec 2020 21:55:18 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644e50ff0ec7c9bc0d471d620940c8ab0fb5ab5eab2580c4bfbe32a5b59b1c7f`  
		Last Modified: Wed, 09 Dec 2020 21:58:16 GMT  
		Size: 97.2 MB (97210571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be8e8008e6d14c6bf974eb5147ebcdfef3df5ffb8e87d501a374af3b43a3c7a`  
		Last Modified: Wed, 09 Dec 2020 21:56:30 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
