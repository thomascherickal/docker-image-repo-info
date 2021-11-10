## `eclipse-temurin:16-jdk-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:f0d21fe326cb280351a5147c06171c95eb16d731eae9d5dcbef59b456af452f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `eclipse-temurin:16-jdk-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull eclipse-temurin@sha256:87d562558e9c13073076bb2d26cc675e64d09cfed33249d71c5ebc0b67a379b5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3088954505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b07ea80d3901518d010446d2484a3902d0cf430594e02710bea39d7901a8838`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 17:37:18 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Wed, 10 Nov 2021 17:38:59 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_windows_hotspot_16.0.2_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_windows_hotspot_16.0.2_7.msi ;     Write-Host ('Verifying sha256 (b153c6ce102c6f05fd710c4b26c64224b649457613dad4830dcc6b551c0a4b3d) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b153c6ce102c6f05fd710c4b26c64224b649457613dad4830dcc6b551c0a4b3d') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-16' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Nov 2021 17:39:57 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 10 Nov 2021 17:39:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733ae7db810292ca583720d2df07a9e972a05f8ee8ffa7cc4609bd46751373de`  
		Last Modified: Wed, 10 Nov 2021 18:30:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582931efcf0c467527d37c54aac4c8a452d88ab6814ab864f5dc5b3347634843`  
		Last Modified: Wed, 10 Nov 2021 18:37:26 GMT  
		Size: 378.9 MB (378900217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0419ff2008a5b7409850014d9d541b99dc8b4b5b00d7c898aeab55aa8321e551`  
		Last Modified: Wed, 10 Nov 2021 18:30:43 GMT  
		Size: 3.9 MB (3928927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afde2849c3f8bb447a088e9460504b0925e3186c7185c762c742e2f2d04267d2`  
		Last Modified: Wed, 10 Nov 2021 18:30:39 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:16-jdk-windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull eclipse-temurin@sha256:9d3b080450e64e0e6d7c137c3a6d34613fb4f1151931ca2b1bce722af2435254
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 GB (6655855764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:716c5836c7720d448c5370f73c312237025f8603153f9de7f289362a5cc61b84`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 17:41:08 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Wed, 10 Nov 2021 17:42:59 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_windows_hotspot_16.0.2_7.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_windows_hotspot_16.0.2_7.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (b153c6ce102c6f05fd710c4b26c64224b649457613dad4830dcc6b551c0a4b3d) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b153c6ce102c6f05fd710c4b26c64224b649457613dad4830dcc6b551c0a4b3d') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-16' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Nov 2021 17:43:57 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 10 Nov 2021 17:43:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53bfa439b18ee70c1022bae0817d89b17c15d777c05339d333ab64c435ebd1e`  
		Last Modified: Wed, 10 Nov 2021 18:38:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50574974ca4ec5ea6df20fdf4c12a34ca26de327c8d003dc4cb601cb967340d7`  
		Last Modified: Wed, 10 Nov 2021 18:45:07 GMT  
		Size: 378.8 MB (378836723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9070024de41f8668ab58495f50c63f2d85310ef6dbc0fbc8aaa5495eef0d26f`  
		Last Modified: Wed, 10 Nov 2021 18:38:21 GMT  
		Size: 3.9 MB (3923913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c66896d4d75f60b7146ce00383ffe98a2725a1dede3267e94412cf08bfdab65`  
		Last Modified: Wed, 10 Nov 2021 18:38:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
