## `adoptopenjdk:11-jdk-openj9-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:b684d239bac8f0bac0738771044987ce14b6265e1ce57efb9e4d8a8d3a6806ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `adoptopenjdk:11-jdk-openj9-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull adoptopenjdk@sha256:33464a99428a26b07e38e57c72a5a489c956b72d60c5eeb63409be8ee8d9ab86
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3068055070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b54da9cb9b0cb5f348860088fbdbc2f7ea03a28060539eb8702c4550812176b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 19:29:28 GMT
ENV JAVA_VERSION=jdk-11.0.11+9_openj9-0.26.0
# Wed, 11 Aug 2021 19:31:23 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.11_9_openj9-0.26.0.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.11_9_openj9-0.26.0.msi ;     Write-Host ('Verifying sha256 (c4eee9cb72f5abd6ccacfcc565415c424f0f2ae32abca159096995a892ccfe6e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'c4eee9cb72f5abd6ccacfcc565415c424f0f2ae32abca159096995a892ccfe6e') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 Aug 2021 19:31:27 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 11 Aug 2021 19:31:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e88a94af3ddf0018d2dead3e9901436b6544ff60a1a8afd374f3d7bce1f2bcd`  
		Last Modified: Wed, 11 Aug 2021 20:40:23 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924cbe51b970f84acf63816d3edea72f875780b6acf301f9306499290a3c2a86`  
		Last Modified: Wed, 11 Aug 2021 20:40:51 GMT  
		Size: 382.1 MB (382051412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e072b928260555f49a26fe50dca2041f4c0107dbb686a266af37af4684330f4`  
		Last Modified: Wed, 11 Aug 2021 20:40:22 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bc66edbd217c3b43aedac7ca3545a6b3fa37741332f105aa5d3de4f191e7e4`  
		Last Modified: Wed, 11 Aug 2021 20:40:22 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jdk-openj9-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull adoptopenjdk@sha256:c06395dcbb7e768c9a5a446442e875b5717b622f4600b98122f53279c8e94567
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 GB (6652955801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90841a2413947f453149c991e50a6b701ef0741e6aafbe34f999820b09163a5b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 19:31:40 GMT
ENV JAVA_VERSION=jdk-11.0.11+9_openj9-0.26.0
# Wed, 11 Aug 2021 19:34:05 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.11_9_openj9-0.26.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.11_9_openj9-0.26.0.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (c4eee9cb72f5abd6ccacfcc565415c424f0f2ae32abca159096995a892ccfe6e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'c4eee9cb72f5abd6ccacfcc565415c424f0f2ae32abca159096995a892ccfe6e') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 Aug 2021 19:34:08 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 11 Aug 2021 19:34:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3752b580a39de8aa4bffd1ecd6cb03b8dcdd395dcabd13e68f0cccb782af22bd`  
		Last Modified: Wed, 11 Aug 2021 20:41:04 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81c180ecdc284a8b151fb0fa616d9c0646c0608fed79d0b24ee36662d06853f`  
		Last Modified: Wed, 11 Aug 2021 20:41:32 GMT  
		Size: 382.0 MB (381984126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ea69a4965f2fe11355cb240a58a8098b5533831cf963fe04527702add44b35`  
		Last Modified: Wed, 11 Aug 2021 20:41:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eda81f5ca09cff17c07e2757e22a153c4a7ffa1f18294f4999f356e89e3a421`  
		Last Modified: Wed, 11 Aug 2021 20:41:04 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
