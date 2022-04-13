## `eclipse-temurin:18-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:c97a11b5f91d9fc3c7da4bbb0bcb93417c046939194bc4e2660a8f28b49deddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:18-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:73f6a4b1a38d45fd817492279591b4dacf30ccf38dd7339328b3a376826812d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3074192902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5077eb33ecb902c019176f87ac9f81fd2f9e2c058785f4c7a4625c176b386109`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 15:44:17 GMT
ENV JAVA_VERSION=jdk-18+36
# Wed, 13 Apr 2022 15:46:06 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_x64_windows_hotspot_18_36.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18%2B36/OpenJDK18U-jdk_x64_windows_hotspot_18_36.msi ;     Write-Host ('Verifying sha256 (28280dd5453a252d412894c9a5b5bcf84ea426a9ecc20135f791f3875b73f343) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '28280dd5453a252d412894c9a5b5bcf84ea426a9ecc20135f791f3875b73f343') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-18' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Apr 2022 15:46:59 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 13 Apr 2022 15:47:00 GMT
CMD ["jshell"]
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
	-	`sha256:56a521912ba5bca01411d0c82d3d0464b55cc650af30cf76bdbd6e585aa56421`  
		Last Modified: Wed, 13 Apr 2022 16:37:17 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00b9289b188fe603a431333b9726c3f5478d74c838098df1a52d448ed00381e`  
		Last Modified: Wed, 13 Apr 2022 16:37:45 GMT  
		Size: 354.5 MB (354472159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69540ef5d1a75e7c8841aeb5e6398642eb36fd58225dfc69422c10ce13a84b1d`  
		Last Modified: Wed, 13 Apr 2022 16:37:18 GMT  
		Size: 3.8 MB (3796301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de2d0f5aea5e9339c2a28e0d9bc95411946d6da997e5adb4338340fe95e0874`  
		Last Modified: Wed, 13 Apr 2022 16:37:16 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
