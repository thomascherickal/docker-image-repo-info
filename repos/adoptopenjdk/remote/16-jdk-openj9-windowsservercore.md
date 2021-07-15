## `adoptopenjdk:16-jdk-openj9-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:d030be4a36dfc0e10269e888b858fd62c52a2019397d37c0c99726fec35b646b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `adoptopenjdk:16-jdk-openj9-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull adoptopenjdk@sha256:3fa19b7f17b53742aea22dd4e24d2ee4443505b626ec1f83f81c454c8e75af67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3075724026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed493b9b4207d98bf325d5e9beee28e7b19c854f180978d06d68fd93f971a146`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 16:25:35 GMT
ENV JAVA_VERSION=jdk-16.0.1+9_openj9-0.26.0
# Wed, 14 Jul 2021 16:27:33 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jdk_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jdk_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi ;     Write-Host ('Verifying sha256 (3aac3769355c1a427947705ef56ff8fcb5d412fdc3afc82c0778a92e643d6303) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '3aac3769355c1a427947705ef56ff8fcb5d412fdc3afc82c0778a92e643d6303') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jul 2021 16:27:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 14 Jul 2021 16:27:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0631565fbd0fcfe16289211cb49dd26166e8301b52595465bf804634a2702efc`  
		Last Modified: Wed, 14 Jul 2021 17:28:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74db1d8982371eb26b8e80886b27f1e3b3c7776b3314c46c150a5455d1ddb476`  
		Last Modified: Wed, 14 Jul 2021 17:36:00 GMT  
		Size: 390.3 MB (390271528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16707398989afd0c7a90c02ffcc86920df34d92ce0cb1c42ccf006569052fc5`  
		Last Modified: Wed, 14 Jul 2021 17:28:42 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1a96181599d3038a768e722f030e434384424c4e1a4cfe38ebcb5b3ac07784`  
		Last Modified: Wed, 14 Jul 2021 17:28:42 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16-jdk-openj9-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull adoptopenjdk@sha256:62e989c55630999f9295129b171694012bf5f1badd22dd184a10f2070281ef5a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 GB (6664289967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333817b0ab2e5c35d32c997e8b8f6ae748068e9601c549217c2c628621830bdd`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 16:27:48 GMT
ENV JAVA_VERSION=jdk-16.0.1+9_openj9-0.26.0
# Wed, 14 Jul 2021 16:30:36 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jdk_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jdk_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (3aac3769355c1a427947705ef56ff8fcb5d412fdc3afc82c0778a92e643d6303) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '3aac3769355c1a427947705ef56ff8fcb5d412fdc3afc82c0778a92e643d6303') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jul 2021 16:30:39 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 14 Jul 2021 16:30:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819e49aed987abe67c0f6c1c20e31746a56bc001e6308314fe98dfaf0987ac04`  
		Last Modified: Wed, 14 Jul 2021 17:36:16 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba65a0af20d261e9b34940ab024ba6a3c12252cd48d954e71aa72b58a7b4fd3`  
		Last Modified: Wed, 14 Jul 2021 17:43:53 GMT  
		Size: 394.7 MB (394652297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2919c839abd3f3c1349b5fbb110c25b5e569eb9d9f03f769ef8503bbd6deeb5a`  
		Last Modified: Wed, 14 Jul 2021 17:36:16 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0953e13a17b6a6a4e5dae5e8953112b286db4d6fe5ba9a220a17e2ed843eb7d5`  
		Last Modified: Wed, 14 Jul 2021 17:36:17 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
