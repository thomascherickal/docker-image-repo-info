## `openjdk:11-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:2b6e38bdca1f53f056a4bd0fddfc691872a6f50b9b023be766d3dcdf33bea9e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `openjdk:11-jdk-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull openjdk@sha256:2a5cf23b640fe496da9c0643c57d118363d0c83e93b54abbae6bb4bcae4fabdb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2578688458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef94fd70f7ad40a6c9f31395da98e8044f5e9e48a49f86c9611f72e1116ae7b`
-	Default Command: `["jshell"]`
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
# Thu, 22 Oct 2020 23:21:48 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9%2B11/OpenJDK11U-jdk_x64_windows_11.0.9_11.zip
# Thu, 22 Oct 2020 23:23:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 22 Oct 2020 23:23:18 GMT
CMD ["jshell"]
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
	-	`sha256:d76cc90f5e6fd588a2e438e4548499fa9010d6d87a141f556dc763a010c57549`  
		Last Modified: Thu, 22 Oct 2020 23:36:21 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a051603998b88f8bf71b1cd3333337f12aaa31ce1b7fdec8cbf40f4e1341be6`  
		Last Modified: Thu, 22 Oct 2020 23:36:39 GMT  
		Size: 195.4 MB (195363302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3832fecd472e5572c66ac541c0d7a58a9638ed36bedcbec61bbdbf88959735b7`  
		Last Modified: Thu, 22 Oct 2020 23:36:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
