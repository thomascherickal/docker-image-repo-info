## `adoptopenjdk:8-jdk-hotspot-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:a8fe70f7e16ed72742b70eee753a134765a7bcb3c76853abb137b5b59a180edb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `adoptopenjdk:8-jdk-hotspot-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull adoptopenjdk@sha256:da86a3c75f10fc77c00591e14a516f7944895e9d965d6971b5499bf372543a8e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5939101579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0f6fa3e584fcb93ba05bb0ba6e7c7b703fba5bfbec6cb7766f289ab1f9bc044`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 22 Jul 2020 13:07:07 GMT
ENV JAVA_VERSION=jdk8u262-b10
# Wed, 22 Jul 2020 13:09:31 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_x64_windows_hotspot_8u262b10.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10/OpenJDK8U-jdk_x64_windows_hotspot_8u262b10.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (251429e9c5ea2d2950aceca10c67e4bf5be3f5f299f2fad4c9757b5ac857cc2c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '251429e9c5ea2d2950aceca10c67e4bf5be3f5f299f2fad4c9757b5ac857cc2c') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370c95b2c779075c70cdf7dc79626aeb314b359ac7544cc6c6d8e27badf5c0f3`  
		Last Modified: Wed, 22 Jul 2020 13:45:03 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9201780d2ba901aa06c2fcb5977e0a190cad4928390cce95a5cfbff41d891e82`  
		Last Modified: Wed, 22 Jul 2020 13:45:21 GMT  
		Size: 201.6 MB (201637206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
