## `openjdk:11-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:35ebf3591ddde847d2c5955ea201cfbacb1c2b39a519041f84c2b67f2956cd52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:11-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:ac4c9cab01e69a870cd1e2660ec691c68aff36e339caf58c70425fa77701b6c4
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2513979659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0100aa5a444edf08af37c5906900607a656f48d93a0128a444fce68853f37d61`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 02:14:08 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 15 Jul 2020 02:14:56 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 15 Jul 2020 02:14:58 GMT
ENV JAVA_VERSION=11.0.7
# Wed, 15 Jul 2020 02:14:59 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.7%2B10/OpenJDK11U-jdk_
# Wed, 15 Jul 2020 02:15:00 GMT
ENV JAVA_URL_VERSION=11.0.7_10
# Wed, 15 Jul 2020 02:16:42 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 02:16:43 GMT
CMD ["jshell"]
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
	-	`sha256:5fe72f810946627936fb3059295f72a1745bfc735925259534b9cee6d7543ae4`  
		Last Modified: Wed, 15 Jul 2020 02:49:46 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f857dc923b786b18ab0918e8a0e201ca958973606bc4e94358acc5f3c1ee1d7`  
		Last Modified: Wed, 15 Jul 2020 02:49:49 GMT  
		Size: 9.1 MB (9135283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad0b70bcbb636fc71c8e95bd0f4843df41e85e883632f29e5ebd34690a8842f`  
		Last Modified: Wed, 15 Jul 2020 02:49:43 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb553b9493c71165c12719d70e33bced3894498fbea8e9ac018d497751060958`  
		Last Modified: Wed, 15 Jul 2020 02:49:43 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6467a3f806183bab739a41e8de2b9f7833db7d9951b02f945888a8c1023b32`  
		Last Modified: Wed, 15 Jul 2020 02:49:43 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a265fdc01ade117a0da41ed1cc89155abb6a4281d2c201b621ae77614c737f`  
		Last Modified: Wed, 15 Jul 2020 02:50:06 GMT  
		Size: 194.6 MB (194645276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0fed61fc7376aabd437d05b6dd14de7453a23625975cf1247e0f3fe2501324`  
		Last Modified: Wed, 15 Jul 2020 02:49:43 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
