## `eclipse-temurin:8u312-b07-jre-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:ddcb9444cd1bbfb74ad916d14ecb1712d54a15136469baaa9aa7d4a067673f95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `eclipse-temurin:8u312-b07-jre-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull eclipse-temurin@sha256:26c6c8284fe56ec230b38486372df2c33c366f7e3ca2980893bf7be6e9819d9a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2777067191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d698002082206fa215723a6ac4184077981b5c08955815a43d0563cbe5a1ee0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 17:10:53 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 10 Nov 2021 17:18:52 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_windows_hotspot_8u312b07.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_windows_hotspot_8u312b07.msi ;     Write-Host ('Verifying sha256 (97bfd53103e4bb8ae317c52e959e2532230d23f17af741a836490884c759b285) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '97bfd53103e4bb8ae317c52e959e2532230d23f17af741a836490884c759b285') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Nov 2021 17:19:43 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5c05b969eb57ff01ac4e9579bfdd1f8a323f61c25a28dbe805cd759dd3f402`  
		Last Modified: Wed, 10 Nov 2021 18:01:27 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8b8054cb058dedc2b8e9c5988094783f46e71ced342956928e6ee524e97798`  
		Last Modified: Wed, 10 Nov 2021 18:07:31 GMT  
		Size: 70.6 MB (70613975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d318b4a33340034ee2837acd35e8991273d925df30bea544b9c9ff27d5b2adab`  
		Last Modified: Wed, 10 Nov 2021 18:06:15 GMT  
		Size: 329.3 KB (329252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
