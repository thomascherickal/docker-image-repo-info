## `adoptopenjdk:8u292-b10-jdk-openj9-0.26.0-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:3b9771d52ab9b9fa56162469200b82f0b61e5ad33951fc1cb13951bc7604b708
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `adoptopenjdk:8u292-b10-jdk-openj9-0.26.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull adoptopenjdk@sha256:7fe77b8198c114e8286a5109e41081e28fafb0e88574a8e784a3fe1a64997b21
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6490643433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8387de524ca253daf537c2c5e58abb960af814e63d6121a262baae48cf18f9f6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 00:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 17:31:03 GMT
ENV JAVA_VERSION=jdk8u292-b10_openj9-0.26.0
# Wed, 15 Sep 2021 17:32:22 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_x64_windows_openj9_8u292b10_openj9-0.26.0.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (49e59ddbf8d9bcffbfe7c02bc4911ccc44b2426db4f4f02a3c13c3c0dadc28df) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '49e59ddbf8d9bcffbfe7c02bc4911ccc44b2426db4f4f02a3c13c3c0dadc28df') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 15 Sep 2021 17:32:24 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8721f004192f15fe71b8626ef3f3e34cbf2cfe1d15a63b6b544ab946162ef707`  
		Last Modified: Wed, 15 Sep 2021 01:10:18 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12828ba3669322416832999f3b6e63fb3363650bf65f0f33e874f448b39148c4`  
		Last Modified: Wed, 15 Sep 2021 18:09:14 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830e15a9bdb80e4dedb8d82bcf09e8110f3a524e5a4b5c1a5fda3e5dc351f792`  
		Last Modified: Wed, 15 Sep 2021 18:09:32 GMT  
		Size: 219.3 MB (219311141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8660a75febd5c98263e9ddd207bc4d39b7c577f86e15840670bba13d4fc1b921`  
		Last Modified: Wed, 15 Sep 2021 18:09:14 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
