## `openjdk:11-jre-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:a57d3564b3e3932a304082d52896b6409acde99bae521f9f0b543e1785230219
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `openjdk:11-jre-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull openjdk@sha256:cf20dca3036a9f843c67b22efa2b916a423db4b5d385efabf0f988ca5561b9e8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5796263387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1fc593e19016348815ab00c347f33dc5e60bb5860ac714bd251b36145ed291`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 02:16:53 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 15 Jul 2020 02:18:26 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 15 Jul 2020 02:18:27 GMT
ENV JAVA_VERSION=11.0.7
# Wed, 15 Jul 2020 02:24:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jre_
# Wed, 15 Jul 2020 02:24:17 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Wed, 15 Jul 2020 02:26:41 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
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
	-	`sha256:47f6d4495790b9ffe933ed4c10a93a72ea2e73c78561ec63e187ec5e21165b51`  
		Last Modified: Wed, 15 Jul 2020 02:50:38 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28651adb0885f4ada774345c2095e6e4849545316eda9ff08da7168e2ce3361a`  
		Last Modified: Wed, 15 Jul 2020 02:50:40 GMT  
		Size: 9.8 MB (9847925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5e5cafd39da68faf0e91257a4f00eb84396541923a5181ecb4be9ef757a81b`  
		Last Modified: Wed, 15 Jul 2020 02:50:34 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc86b98d589453126a8791c0e343a12d74ffea9691d2948a6492172df258d25`  
		Last Modified: Wed, 15 Jul 2020 02:52:43 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e834bddb8fcd3ee964e8ed0e44347a99a0c9179f5f2490df655e2576004c328`  
		Last Modified: Wed, 15 Jul 2020 02:52:42 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e2c259f1333ef93c53556a6c36944582e59818134c739a3eb212c2aa2356d9`  
		Last Modified: Wed, 15 Jul 2020 02:52:52 GMT  
		Size: 48.9 MB (48947723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
