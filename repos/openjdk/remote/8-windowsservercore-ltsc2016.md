## `openjdk:8-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:e63c8227620720394c75bb508d1d09bea6fa596efe1301948f767717dfa89612
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `openjdk:8-windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull openjdk@sha256:34da86101369dd0a9cc74a696c3f0a38cb5eb0f22d094cd68188dd660162028b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5857990481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61b5a1709fc5cf5e1a481bd36c2219590ff7b021816952932dcb2b05275d0126`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Aug 2020 20:31:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 15:58:10 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 12 Aug 2020 15:59:22 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 12 Aug 2020 15:59:23 GMT
ENV JAVA_VERSION=8u265
# Wed, 12 Aug 2020 15:59:24 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jdk_x64_windows_8u265b01.zip
# Wed, 12 Aug 2020 16:01:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac -version'; javac -version; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:32838d9637dc39d4acee78700b0f93d6c8c9d2db755f12c8009c1b51687d3fbd`  
		Last Modified: Tue, 11 Aug 2020 20:54:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2785dc5ba8107135b4e1c3a8709ebe4838c24deab58b743d2dd94ec05eee2881`  
		Last Modified: Wed, 12 Aug 2020 16:22:51 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484711f5757749de8c97caa8f632d669911c1bb5c6a31eb08123e3e3a89221d9`  
		Last Modified: Wed, 12 Aug 2020 16:22:54 GMT  
		Size: 9.9 MB (9869230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d66838d1245feb00bdbd58ac1bbeb128973bcf5570fdef979801d7f55394867`  
		Last Modified: Wed, 12 Aug 2020 16:22:50 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff802fd43b8af680ab994a6baa30096988a924aec1aac579db0149689ed27cc`  
		Last Modified: Wed, 12 Aug 2020 16:22:51 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10deabcd5204c66b786895ca85eccbbc201ad5666d38a503085646c096e608c`  
		Last Modified: Wed, 12 Aug 2020 16:23:11 GMT  
		Size: 110.0 MB (109969181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
