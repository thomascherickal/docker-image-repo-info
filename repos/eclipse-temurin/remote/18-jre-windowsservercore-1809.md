## `eclipse-temurin:18-jre-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:6b8638d5f10fe7082073e1d2d958126097d4d7139c8015adb9f02cf9b2fc59f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:18-jre-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:4064651d5383b627c2f24823ba074c50c95d60009519dbccfcb37193a5259f83
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2793203535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aba031841a8533fd83945bfde6c45852f3ac7c699bec94fece15a325916e38d9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 04 May 2022 18:19:50 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 04 May 2022 18:26:17 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_windows_hotspot_18.0.1_10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_windows_hotspot_18.0.1_10.msi ;     Write-Host ('Verifying sha256 (75a0749dfdec3f7238b0ba2572ff9b2f7debbb56710531b960d60769b1b070f5) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '75a0749dfdec3f7238b0ba2572ff9b2f7debbb56710531b960d60769b1b070f5') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-18' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 04 May 2022 18:27:15 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d124a9534d8e82e1fdab3593775156cb0a6c44cb1842c7050a417f8876da216`  
		Last Modified: Wed, 04 May 2022 18:32:47 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5784cc3c661e2970063a20d03774aae304630e6418859e45c0a279d9cedc11ba`  
		Last Modified: Wed, 04 May 2022 18:35:36 GMT  
		Size: 74.1 MB (74089950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a30d4a4d620fed975fb96ce464661a29dea3ae291929ed1460f9d65a7d3148f`  
		Last Modified: Wed, 04 May 2022 18:35:27 GMT  
		Size: 3.2 MB (3190412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
