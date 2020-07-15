## `openjdk:8u252-jdk-windowsservercore`

```console
$ docker pull openjdk@sha256:8c65ca3671565d42d286a8595d40ad66f8e30982d19e8c7418367f5c2548c9d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `openjdk:8u252-jdk-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:70342662a936e41adf4a224581b6185b5c120619f9ee9e6fabcedb4be3433251
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2423748173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee27d28107269896e5bc2c6c6c7a766bf4f7a9852417d27cfb1e7af9082042af`
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
# Wed, 15 Jul 2020 02:28:15 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Wed, 15 Jul 2020 02:28:17 GMT
ENV JAVA_URL_VERSION=8u252b09
# Wed, 15 Jul 2020 02:29:38 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac -version'; javac -version; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
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
	-	`sha256:23f100882d78aaf1ebca854a82d7aac838c6d189c7353322eff59e0c92c18dee`  
		Last Modified: Wed, 15 Jul 2020 02:53:28 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadf6a75c5fd82996ffa2ac9b2aa63f890c416d8c187297773765dbb231771eb`  
		Last Modified: Wed, 15 Jul 2020 02:53:28 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607966cf038175a59f9886216563d4d381c330bf675e4ed4427bfd68628dcfa3`  
		Last Modified: Wed, 15 Jul 2020 02:53:41 GMT  
		Size: 104.4 MB (104414877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8u252-jdk-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull openjdk@sha256:7782ebdf8635067155793eb6eb35ed2cbabe30ba36cb8754d230d07064a53e2a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5856880283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27c5afd324e2524cab20c89624d1813c7fdca1cdffdadf8921eb6d0243a63948`
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
# Wed, 15 Jul 2020 02:31:29 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u252-b09/OpenJDK8U-jdk_
# Wed, 15 Jul 2020 02:31:31 GMT
ENV JAVA_URL_VERSION=8u252b09
# Wed, 15 Jul 2020 02:33:51 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac -version'; javac -version; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
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
	-	`sha256:13e011b2caf5c7b955215e7b1f5b50f9ad529cad1a8e7c9fcb9d32557c5ac500`  
		Last Modified: Wed, 15 Jul 2020 02:53:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149ac9938eec70456439db474217447b303bd18c27e6db0ea69e2d0606009892`  
		Last Modified: Wed, 15 Jul 2020 02:53:58 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35042e0c2863127a190bb9f36a71b1c3062ea5ef74c32ebee1f2b71e28f94544`  
		Last Modified: Wed, 15 Jul 2020 02:54:12 GMT  
		Size: 109.6 MB (109563950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
