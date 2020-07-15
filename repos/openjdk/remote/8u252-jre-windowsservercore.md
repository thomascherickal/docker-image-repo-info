## `openjdk:8u252-jre-windowsservercore`

```console
$ docker pull openjdk@sha256:00f602dbcd263815a6e63157448202e2f253ae8fced6b03dd5d8c844254dc272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `openjdk:8u252-jre-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:98fa42a1653d561ebef5f10c4d8f6a0cbf0d48b144471ae8a9aa35c80dd59a45
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2361421905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:011a2571fb6d5b086e614a37973f7c9982dfab9d4273576393a0bca459f0b00a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 02:27:30 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 15 Jul 2020 02:28:13 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 15 Jul 2020 02:28:14 GMT
ENV JAVA_VERSION=8u252
# Wed, 15 Jul 2020 02:35:21 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Wed, 15 Jul 2020 02:35:22 GMT
ENV JAVA_URL_VERSION=8u252b09
# Wed, 15 Jul 2020 02:36:15 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df9d9d4f1a50ee68e53390188a27d433831832a28f411a3139d70477d10675d`  
		Last Modified: Wed, 15 Jul 2020 02:53:31 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9cc415e666896862859052aa477e1be3eacd38ff9d000d097e03995c2b6b50`  
		Last Modified: Wed, 15 Jul 2020 02:53:31 GMT  
		Size: 9.1 MB (9135307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff5bceb5d0895ccb6ea2cf649ecc9c9e65e7ed9b082f3dac650d4c3e99a0089`  
		Last Modified: Wed, 15 Jul 2020 02:53:28 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430968f1f53814f19b01589303f70ab38f3f3aea714c0e4f684ad620fea61adb`  
		Last Modified: Wed, 15 Jul 2020 02:54:53 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582d222e91f94181a099f8eb3af1de28e9ae7a574cb478bdd123737e195cf7db`  
		Last Modified: Wed, 15 Jul 2020 02:54:53 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3df1299c230c4cfed1d069670f58687c48ae0bd5eea037c0248e05a3f0c64b`  
		Last Modified: Wed, 15 Jul 2020 02:55:00 GMT  
		Size: 42.1 MB (42088686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8u252-jre-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull openjdk@sha256:38126e33a859f06b3673ba0651ac645d634544340cc67ba9170cd5960893681a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5794555969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0c4e91dca0c4b4474d9174cd15e80da1ede7305d7eda759e444a0f68a5c627`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 02:29:56 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 15 Jul 2020 02:31:27 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 15 Jul 2020 02:31:28 GMT
ENV JAVA_VERSION=8u252
# Wed, 15 Jul 2020 02:36:22 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jre_
# Wed, 15 Jul 2020 02:36:23 GMT
ENV JAVA_URL_VERSION=8u252b09
# Wed, 15 Jul 2020 02:38:18 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a507ee4c5f1710265ef802239c6b751e4038de0880d1199939f60e9a55b852`  
		Last Modified: Wed, 15 Jul 2020 02:54:02 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f508a80c49db228b8b105873dc5f16dcab73be484890fc688db12a14646d0b9e`  
		Last Modified: Wed, 15 Jul 2020 02:54:01 GMT  
		Size: 9.8 MB (9848518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb57449db94f282f29d3b41741b7b624399cb9fc753ccbbe77da93115440bdc5`  
		Last Modified: Wed, 15 Jul 2020 02:53:59 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fd05cc4cdffe0615b2958724fd2d1581bf3f19aae24b2830c92ead8aac09dc`  
		Last Modified: Wed, 15 Jul 2020 02:55:13 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3ab1aaddc82af85a9540c58409dff1144c7941bca256fbc0958a6f97f2459d`  
		Last Modified: Wed, 15 Jul 2020 02:55:13 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71c58a6907ef52618c608c63ba949b46e8568dbaa1324182002085fdef58996`  
		Last Modified: Wed, 15 Jul 2020 02:55:21 GMT  
		Size: 47.2 MB (47239691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
