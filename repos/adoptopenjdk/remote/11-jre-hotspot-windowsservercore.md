## `adoptopenjdk:11-jre-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:f4956a3695567f75548a6bf4b50754ddebafb165057a12ae9a1a77aa3d12d4d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `adoptopenjdk:11-jre-hotspot-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull adoptopenjdk@sha256:7f19226df5de5e90728a6052da9079a2756e5773cb814c05f4a95bdcebcad121
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2759188563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52a57927a321f6a428ad8f5398ff961c365afaa08204c6b8559df25ed403ac43`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 18:54:37 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Wed, 11 Aug 2021 19:00:55 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.11_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.11_9.msi ;     Write-Host ('Verifying sha256 (d52262a1ac6d86326cd071b687dcc5bb546bedda6d03c6bd26a046070a013df3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'd52262a1ac6d86326cd071b687dcc5bb546bedda6d03c6bd26a046070a013df3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:a771911218e2373e9fb4e1fd731e5b0e16b600b45f6ac384375ded412a3ae225`  
		Last Modified: Wed, 11 Aug 2021 20:00:00 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c103c68691ac5288a913c45b39f356dfdd01bff91f66b99b8e63e7cd9335d4e5`  
		Last Modified: Wed, 11 Aug 2021 20:15:46 GMT  
		Size: 73.2 MB (73187795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jre-hotspot-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull adoptopenjdk@sha256:18a04b7a655eda26979ec6128b9b949b74c8aa3b1fd0b84fec876aa03408b996
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6344083922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfffb17e42dd1737c3c3a89bd1aa06e58deab444c4b0119e49586ebf611aab7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 18:56:49 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Wed, 11 Aug 2021 19:03:08 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.11_9.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jre_x64_windows_hotspot_11.0.11_9.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (d52262a1ac6d86326cd071b687dcc5bb546bedda6d03c6bd26a046070a013df3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'd52262a1ac6d86326cd071b687dcc5bb546bedda6d03c6bd26a046070a013df3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:aa8039775f56cdcb7aca9dac0ddee754bded399b4e429e1e7a758cc5c329d05f`  
		Last Modified: Wed, 11 Aug 2021 20:07:24 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad82924b35720b7c72b3e8c44bff5948645c07deead5b31ff12caf6b155ea12`  
		Last Modified: Wed, 11 Aug 2021 20:17:24 GMT  
		Size: 73.1 MB (73115066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
