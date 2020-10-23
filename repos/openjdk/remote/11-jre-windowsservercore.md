## `openjdk:11-jre-windowsservercore`

```console
$ docker pull openjdk@sha256:34ebaf05e33d5d46c794c87b5a0a9e15a4523e98034690d39b5d19da2fab5319
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `openjdk:11-jre-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull openjdk@sha256:e1284e501a9da4bf47b18792bbe8532b58afe0755add2b88d76a1d0295b381c7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2427348022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbcd4d3cc8f7df8c3e50c82561de6510405bdf4e413d55ca37e00022fecfb75c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 18:03:11 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 14 Oct 2020 18:03:57 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Thu, 22 Oct 2020 23:21:47 GMT
ENV JAVA_VERSION=11.0.9
# Thu, 22 Oct 2020 23:27:23 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9%2B11/OpenJDK11U-jre_x64_windows_11.0.9_11.zip
# Thu, 22 Oct 2020 23:28:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f24549ffd67841d2abd5b00ca5ac77dd540ae7fdd1c5015df4b2e75feb1c873`  
		Last Modified: Wed, 14 Oct 2020 18:40:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1117af659dc8efb682205f3b9eeb244de0c062c1c510b5edfe0c1fb95679113f`  
		Last Modified: Wed, 14 Oct 2020 18:40:09 GMT  
		Size: 9.2 MB (9229357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c17afe9ab1d9f7aaa2f8fbb9c9cd9d4744b368ba4193cb4ca54a79980f9669d`  
		Last Modified: Thu, 22 Oct 2020 23:36:20 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34de181da77371113fdaa237fbb85872fce6c280f2acdd28d00e6c9abf05ecfc`  
		Last Modified: Thu, 22 Oct 2020 23:38:37 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51771593e70ad6e7a3957548aeb3c2e5c71f84982baa09e9d877715e38db8c21`  
		Last Modified: Thu, 22 Oct 2020 23:38:46 GMT  
		Size: 44.0 MB (44023987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-jre-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull openjdk@sha256:f62072b5a60dcfe041df48e6e85c340a5ed5159ae447b80d429e40dfc16d0598
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5800455169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89147e5692b9d79d649998aa5735365dc3e5f38bf6af485efb2a08b5f952e54b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 18:05:40 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 14 Oct 2020 18:06:59 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Thu, 22 Oct 2020 23:23:28 GMT
ENV JAVA_VERSION=11.0.9
# Thu, 22 Oct 2020 23:28:16 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9%2B11/OpenJDK11U-jre_x64_windows_11.0.9_11.zip
# Thu, 22 Oct 2020 23:29:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268572cf853e5b33ed53392bbc6e62b1e762b24c14e02c14f668989d10278072`  
		Last Modified: Wed, 14 Oct 2020 18:44:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3d8ff91d4c7e5d649f483f3fb3c7e2fdcc0f92af4d0de4baa1d52f9ec225ca`  
		Last Modified: Wed, 14 Oct 2020 18:44:26 GMT  
		Size: 9.9 MB (9921487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a8e817ddf946a01ba4f4f2030852f1d4a196ffe23846cf5e5591dd5c9f6961`  
		Last Modified: Thu, 22 Oct 2020 23:37:01 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcafcfa445a1e3f03b49405c34be2dc9ef3610dfc1be75b8ccbf0ebb26b6fc80`  
		Last Modified: Thu, 22 Oct 2020 23:39:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d20014bfbf0791aacdff4f49f90d30ece6a7aa596d976a7f8c54db0c0f6726`  
		Last Modified: Thu, 22 Oct 2020 23:39:58 GMT  
		Size: 49.2 MB (49177421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
