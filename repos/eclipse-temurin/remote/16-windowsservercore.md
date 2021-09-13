## `eclipse-temurin:16-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:0e7a8194723769b98f09c929e910e6f23e7cfc5500696bd1cdcafca6504b5b17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `eclipse-temurin:16-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull eclipse-temurin@sha256:753b289c050f7f87dbb6414aa12f6f0c9c7f317df57de244287366af857b1843
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3068875121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34cfdfd45c65e8dd2fde4a1ef9502531e5bd3f05175141b3a287751073377825`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 16:46:30 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Mon, 13 Sep 2021 18:31:33 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_windows_hotspot_16.0.2_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_windows_hotspot_16.0.2_7.msi ;     Write-Host ('Verifying sha256 (b153c6ce102c6f05fd710c4b26c64224b649457613dad4830dcc6b551c0a4b3d) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b153c6ce102c6f05fd710c4b26c64224b649457613dad4830dcc6b551c0a4b3d') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-16' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 13 Sep 2021 18:32:29 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Mon, 13 Sep 2021 18:32:29 GMT
CMD ["jshell"]
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
	-	`sha256:d7aeace5fc0b6f75f7cbcff6cad178a22d6eb4b66e9199f4398fddf666e9461f`  
		Last Modified: Wed, 25 Aug 2021 23:32:58 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd58ec4ad328f58745ee08de6c4d16434648a9e081c5c9bc723bd5fdad17f926`  
		Last Modified: Mon, 13 Sep 2021 18:55:00 GMT  
		Size: 378.9 MB (378928238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407199e972b86011bebb92cd313ff024552c342be372cbca3870ab6fe6f7894a`  
		Last Modified: Mon, 13 Sep 2021 18:54:29 GMT  
		Size: 3.9 MB (3944737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bb30f68c640480d9ed3dee0981d84f72d226619fb453c36a23bb428e5ab6c8`  
		Last Modified: Mon, 13 Sep 2021 18:54:27 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:16-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull eclipse-temurin@sha256:b0bc4602b2a2ce0e1ffc1acc999be1428e8df9edd86324b6fb8cb27c967d57cf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 GB (6653715602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72337e67ded24fe0590036b7cb0521cf861638d23b72350783155270f19bbeb0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 16:49:10 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Mon, 13 Sep 2021 18:34:30 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_windows_hotspot_16.0.2_7.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_windows_hotspot_16.0.2_7.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (b153c6ce102c6f05fd710c4b26c64224b649457613dad4830dcc6b551c0a4b3d) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b153c6ce102c6f05fd710c4b26c64224b649457613dad4830dcc6b551c0a4b3d') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-16' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 13 Sep 2021 18:35:26 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Mon, 13 Sep 2021 18:35:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34118a1198de824f2a68d546f879aa8137bdbd9ef7c68488df1124af810167f6`  
		Last Modified: Wed, 25 Aug 2021 23:33:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2445cbef047ae664b0e5863eccea34306b5019cb3921558497aaf36576fea4dc`  
		Last Modified: Mon, 13 Sep 2021 18:55:40 GMT  
		Size: 378.8 MB (378832274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ecaa5533b1c7691c5102a078596ec7260a41c232f6e5250488921dd375b5e1`  
		Last Modified: Mon, 13 Sep 2021 18:55:15 GMT  
		Size: 3.9 MB (3913063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4a5f0504e896b1c94f8e01ec29c0685c27798ca166dde977d47b6086850826`  
		Last Modified: Mon, 13 Sep 2021 18:55:13 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
