## `adoptopenjdk:8-jre-openj9-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:1d2adf9b400c9eeaf8d3e35790b52d87ba3b110bb7487114f48cbe2f7527777a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `adoptopenjdk:8-jre-openj9-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull adoptopenjdk@sha256:fb449a7d91c822cf54f57f69a0dc61aec90abde2e01c9f210a3a2f44c28006c3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2565763834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce374fc8c45aeacb929cd2c74d231464d07d682e2e6e94a47037fcfcaac61d2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 10 May 2021 18:39:59 GMT
ENV JAVA_VERSION=jdk8u292-b10_openj9-0.26.0
# Mon, 10 May 2021 18:45:19 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jre_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jre_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ;     Write-Host ('Verifying sha256 (8decae9e065946cfc9a4b7f3c0ed61cfc6fe3076cdcbbbece33ef39c9ccef6e3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8decae9e065946cfc9a4b7f3c0ed61cfc6fe3076cdcbbbece33ef39c9ccef6e3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 10 May 2021 18:45:21 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c2ef53c6a0a5de9e14afebacfd8b9e61d77951aea45bbfd7ed3065fa846dc0`  
		Last Modified: Mon, 10 May 2021 19:33:59 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a18e65f550e3aa42b9c1c3a3143502219981c9357b2b8fb0c41369e74be1b95`  
		Last Modified: Mon, 10 May 2021 19:35:39 GMT  
		Size: 96.0 MB (96005677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43d79722069a7982b7e81db497c1465d65b35949063cb705506ae9e4a94cd49`  
		Last Modified: Mon, 10 May 2021 19:35:26 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-openj9-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull adoptopenjdk@sha256:603ef6701f74944bebb0ce4c4de049c58ed5a168c5c91fbe13085b9a95032afd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5891403256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c032fb0ced8a6c72d540bca470ca0e44e0690441fa4ec51f89f08ea3992dfb48`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 10 May 2021 18:41:42 GMT
ENV JAVA_VERSION=jdk8u292-b10_openj9-0.26.0
# Mon, 10 May 2021 18:47:36 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jre_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jre_x64_windows_openj9_8u292b10_openj9-0.26.0.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (8decae9e065946cfc9a4b7f3c0ed61cfc6fe3076cdcbbbece33ef39c9ccef6e3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8decae9e065946cfc9a4b7f3c0ed61cfc6fe3076cdcbbbece33ef39c9ccef6e3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 10 May 2021 18:47:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df71603d85b19ba77dce29770c6ac50656b491c123087ef6681113fd698e5b07`  
		Last Modified: Mon, 10 May 2021 19:34:42 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a838e76f7c8213283f45239d685a131945b830bb068631b1bc73d98f52e04fc`  
		Last Modified: Mon, 10 May 2021 19:36:03 GMT  
		Size: 96.5 MB (96515117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4938355f42c86882ca08f905bd43e963ef2e15e1bbea496707a5d4bd6b7b2652`  
		Last Modified: Mon, 10 May 2021 19:35:49 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
