## `adoptopenjdk:8-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:e5d7b06bb8121910fc08fc5114448c27134e9b181ab8cffce334c32450d1459f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `adoptopenjdk:8-hotspot-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull adoptopenjdk@sha256:c26914139484152aaeab04e763b7c3391612c701f3ae235d35a8b5bce33c5ca9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2879893451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:099b54d81793efdbdd4f91ed0e9a5b209eb5a16a8c95f8fd776a067cd3578ceb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 17:06:23 GMT
ENV JAVA_VERSION=jdk8u292-b10
# Wed, 15 Sep 2021 17:07:36 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_windows_hotspot_8u292b10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_windows_hotspot_8u292b10.msi ;     Write-Host ('Verifying sha256 (f6bd2e351a451b8dc7ed19d44b18a27ff8a0602016625fac5134c4defe5e560c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f6bd2e351a451b8dc7ed19d44b18a27ff8a0602016625fac5134c4defe5e560c') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a4de21e2555698cee55a4c837cdf4c76050088ebf2a2cb2ea0f1e3fc0763e6`  
		Last Modified: Wed, 15 Sep 2021 17:55:20 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88ffa1cf46e3d9201138864e9a20371076b4b4020c1647b130616eb007c8104`  
		Last Modified: Wed, 15 Sep 2021 17:58:42 GMT  
		Size: 193.2 MB (193192710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
