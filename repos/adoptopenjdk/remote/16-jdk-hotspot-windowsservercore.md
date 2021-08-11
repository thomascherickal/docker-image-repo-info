## `adoptopenjdk:16-jdk-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:3b9f4f0fe42c34f41baa6cb96c461ee4ec56290ed6377aa11acda6d786e0709f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `adoptopenjdk:16-jdk-hotspot-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull adoptopenjdk@sha256:fe935262199cff01f6461cf1de9f944c270099bb29abfc0a8b6c87a2c70d36d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3063966863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7750765deade9d5af600fcce259ff3bde1dcb7d0d80f9b3ea0cf4bd631502ac`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 19:12:17 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Wed, 11 Aug 2021 19:14:11 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_windows_hotspot_16.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_windows_hotspot_16.0.1_9.msi ;     Write-Host ('Verifying sha256 (dc898ec3574e08a90f67fa75808954462749c874ab22c860ded6de051bcc7499) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'dc898ec3574e08a90f67fa75808954462749c874ab22c860ded6de051bcc7499') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 Aug 2021 19:14:14 GMT
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
	-	`sha256:5e24c8c89f41bd2695a9dc52b1094085a6b5692b2ee1702370c80c986a20d380`  
		Last Modified: Wed, 11 Aug 2021 20:26:57 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c98b9b4cbf111fd931d0e918f1ccc673095272314e985406717b3b62281d7c9`  
		Last Modified: Wed, 11 Aug 2021 20:27:25 GMT  
		Size: 378.0 MB (377964646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19be57862606a7e0b77ad87e5c49021acf2fa63924a529c2c0def9183c9a404`  
		Last Modified: Wed, 11 Aug 2021 20:26:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16-jdk-hotspot-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull adoptopenjdk@sha256:b9757d821509a34a2eadff84f0820cb890a2756f0ab7577693dd6c5e0ee1c396
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6648865947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d015a566ea9e5a15eb3582ea12fc9b06860b3365b2cb7b2a51343f1cf431711a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 19:14:30 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Wed, 11 Aug 2021 19:17:01 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_windows_hotspot_16.0.1_9.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_windows_hotspot_16.0.1_9.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (dc898ec3574e08a90f67fa75808954462749c874ab22c860ded6de051bcc7499) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'dc898ec3574e08a90f67fa75808954462749c874ab22c860ded6de051bcc7499') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 Aug 2021 19:17:04 GMT
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
	-	`sha256:3853bc964c0771b394640263a859a030e2abb0cccf58d349d9816d13d7f066b5`  
		Last Modified: Wed, 11 Aug 2021 20:27:42 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985326479726df28ebc161099c63328eabd5f873e1d98cbfbfaf9b9da8dccde5`  
		Last Modified: Wed, 11 Aug 2021 20:28:12 GMT  
		Size: 377.9 MB (377895657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611f40e19fbc368091a994ef44b718bc48286e58080741325622f157acca6206`  
		Last Modified: Wed, 11 Aug 2021 20:27:42 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
