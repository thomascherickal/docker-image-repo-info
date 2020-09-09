## `adoptopenjdk:8u262-b10-jdk-openj9-0.21.0-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:e3e7ba9bf21f02319c64c30b23bd70788c2b0f56d85ceb769a928ceb84d4cc4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `adoptopenjdk:8u262-b10-jdk-openj9-0.21.0-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull adoptopenjdk@sha256:cfe5c8d6d13b503b51b2e0d6568c86dbe5908d65275a3a4b711d146924dc5898
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2576266328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f52d4ae97d2932cd1de6627459073a0ae3d04021fa6da305637331229d60e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 18:33:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 09 Sep 2020 18:35:24 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jdk_x64_windows_openj9_8u262b10_openj9-0.21.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jdk_x64_windows_openj9_8u262b10_openj9-0.21.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (824f32604bee0469d9dac5208dc8a025a142d95c53d838eab753bda619d46614) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '824f32604bee0469d9dac5208dc8a025a142d95c53d838eab753bda619d46614') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Sep 2020 18:35:25 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb9d8bd407e3c9de9e1d4d8123749862863fc8980fa1937385d3aa6660e6344`  
		Last Modified: Wed, 09 Sep 2020 19:30:30 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65431175d2044afb5814a0938fc9fcc4e297b26bee7388819065368f12794fc`  
		Last Modified: Wed, 09 Sep 2020 19:30:50 GMT  
		Size: 225.0 MB (224990693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7a979e64777f10e0566ff5c583743d993d6deed0b18f2b99891c587284fe26`  
		Last Modified: Wed, 09 Sep 2020 19:30:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
