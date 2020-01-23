## `openjdk:8u242-jre-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:e1031f1ba67e9ec9e1bb3533afc0b2001aede990472b0fc111a90d39eeb5587d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `openjdk:8u242-jre-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull openjdk@sha256:3c7b6e1866a63f50776448b628e78181c930242bfb0799fd197292546037e1e0
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772678109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f22a7f5e4545bc776b4cfb9dc87e6353ea83c74841b7b536caa32a34bcc6bfe`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jan 2020 01:33:20 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 15 Jan 2020 01:34:26 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Thu, 23 Jan 2020 00:24:26 GMT
ENV JAVA_VERSION=8u242
# Thu, 23 Jan 2020 00:29:20 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Thu, 23 Jan 2020 00:29:22 GMT
ENV JAVA_URL_VERSION=8u242b08
# Thu, 23 Jan 2020 00:30:49 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64342381c3078746d49b0bd22acdcb54c6ed79741d2dc83408852dbc0f261239`  
		Last Modified: Wed, 15 Jan 2020 02:15:22 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1b90544f2b8fdcf67d90077c3afe669dd4c0e5cd3913aaa2cce71f0b3e8b1b`  
		Last Modified: Wed, 15 Jan 2020 02:15:21 GMT  
		Size: 5.4 MB (5385785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732e4a8ce6e36b30abbd0006d38a48caa5d47b677ee00f48c6342799884154d3`  
		Last Modified: Thu, 23 Jan 2020 00:35:35 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179c3c734fc9f3b4080e8a60ec25058e0653a7f09ceb1b8bd375f4faa29d13b2`  
		Last Modified: Thu, 23 Jan 2020 00:38:32 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b3cc975a4e35e330f91c1edde3e9a1e3d4288074f89456c26fd9d6fe5d0078`  
		Last Modified: Thu, 23 Jan 2020 00:38:33 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79a9a53ef113969f0386dc7d8bf71c08c893b3363d94f4cd4e1e92dbe937cac`  
		Last Modified: Thu, 23 Jan 2020 00:38:41 GMT  
		Size: 42.7 MB (42687053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
