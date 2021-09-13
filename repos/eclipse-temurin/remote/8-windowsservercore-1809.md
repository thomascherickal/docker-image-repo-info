## `eclipse-temurin:8-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:2ccabd188bf8c5fe83d16848841fd891abc4c691d477a5c7d56b373e5f0e03ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `eclipse-temurin:8-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull eclipse-temurin@sha256:71f279383199d100c999501835f8c4282c7751e084b5d1d00dcc03908baf60a4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2875667419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:319b60e4ca5907a2b9f88ad453718db5f1a6a7bd28f38f3e64f05ec15b84d41f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 16:29:13 GMT
ENV JAVA_VERSION=jdk8u302-b08
# Mon, 13 Sep 2021 18:15:22 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08.1/OpenJDK8U-jdk_x64_windows_hotspot_8u302b08.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08.1/OpenJDK8U-jdk_x64_windows_hotspot_8u302b08.msi ;     Write-Host ('Verifying sha256 (fe3546a8e8dd7d4e929028ef3794431748caddf7fc1cf481618e8d6f8aa15427) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'fe3546a8e8dd7d4e929028ef3794431748caddf7fc1cf481618e8d6f8aa15427') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 13 Sep 2021 18:16:23 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf5ffaf540fdab4c73913780b326ca2cb2c5a0f61040fdb1c0e6aeaf9d2f768`  
		Last Modified: Wed, 25 Aug 2021 23:17:07 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187a7abfa9f9a11735941174929044e01185272e0170e245934c21949bb7d336`  
		Last Modified: Mon, 13 Sep 2021 18:41:09 GMT  
		Size: 189.3 MB (189322861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a9ace9f8e83803854248f5db8f1f637ad4ba5c12805cdfe044ef75ed7ca773`  
		Last Modified: Mon, 13 Sep 2021 18:37:41 GMT  
		Size: 343.8 KB (343770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
