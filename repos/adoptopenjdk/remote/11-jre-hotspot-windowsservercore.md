## `adoptopenjdk:11-jre-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:958bb1cf1a4919081b96943ee95775e8181df582d2d136f5281a034c05cfa265
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `adoptopenjdk:11-jre-hotspot-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull adoptopenjdk@sha256:6bba4bb2b9f667dc9c66f7bd43278bc90f6f56578e6ca370b72ef461036f3d08
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2547685992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a750ec2858b33ae60a178252863833da6d3d23bce003c9859237e49a02ee0d92`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 10 May 2021 18:23:01 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Mon, 10 May 2021 18:29:09 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.11_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.11_9.msi ;     Write-Host ('Verifying sha256 (d52262a1ac6d86326cd071b687dcc5bb546bedda6d03c6bd26a046070a013df3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'd52262a1ac6d86326cd071b687dcc5bb546bedda6d03c6bd26a046070a013df3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:54d2093d3e911cf6a5e76917eac57c67658476ee3f28936c082036167c43d451`  
		Last Modified: Mon, 10 May 2021 19:17:53 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741ca97006b5a46dbc9c1b57f641658352f25f0aa6259a25b9d3f8bc7f80a10a`  
		Last Modified: Mon, 10 May 2021 19:27:41 GMT  
		Size: 77.9 MB (77929292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jre-hotspot-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull adoptopenjdk@sha256:86f3fa68ff9f5e58d7af99e6640ec48be94df09e3e0cc49cd4ca3a2322ba92ed
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5873316682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a5a831a3d83c67d2defddb492eb3b7a09cd048e9327b7bf141eaccac6737b76`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 10 May 2021 18:24:58 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Mon, 10 May 2021 18:31:20 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.11_9.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.11_9.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (d52262a1ac6d86326cd071b687dcc5bb546bedda6d03c6bd26a046070a013df3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'd52262a1ac6d86326cd071b687dcc5bb546bedda6d03c6bd26a046070a013df3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:721443176c09d4722c9d6b19e1d63322867afbde1b10ad586fddce013078fa1d`  
		Last Modified: Mon, 10 May 2021 19:25:18 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccc344ea82d1bf4d5028119383c98e01cc6e119e95a317236fe787c11ab8522`  
		Last Modified: Mon, 10 May 2021 19:28:06 GMT  
		Size: 78.4 MB (78430009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
