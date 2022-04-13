## `eclipse-temurin:8-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:77075dcc3e160d5810d176d10f351e45622385c266729891558d3159a2066d3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:8-jdk-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:51bbe8a2762291bd1cfaf6b869491f81f339663bac29138be3ee0af8ac575053
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2905654243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:747322c530d35585f204271b6eb6660d6f3d38ce5a7c93f13d6f9220ec4ef163`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 15:13:43 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Wed, 13 Apr 2022 15:15:02 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_windows_hotspot_8u322b06.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_windows_hotspot_8u322b06.msi ;     Write-Host ('Verifying sha256 (e9337d5bba9b60a9d00a939fecb05718b2303023a587da6ae4862080714f9f0b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e9337d5bba9b60a9d00a939fecb05718b2303023a587da6ae4862080714f9f0b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Apr 2022 15:15:58 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:0cda3f8877932a5001b8f1e44d7fc68f233d50da7e29742e9b26a24f99f161fd`  
		Last Modified: Wed, 13 Apr 2022 15:57:34 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97734b51099941a2210d38ef1d36cb6212e9aa14b550ba56c9850fac11b813e8`  
		Last Modified: Wed, 13 Apr 2022 15:57:50 GMT  
		Size: 189.4 MB (189401053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b1b560c16c90b2b08c13247968ddb865042f591f3191af5efccdc1e0e7fdc7`  
		Last Modified: Wed, 13 Apr 2022 15:57:35 GMT  
		Size: 330.2 KB (330155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
