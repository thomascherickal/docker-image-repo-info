## `openjdk:11-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:671ab3b6d3b409d2ca471d93aec06d23d7ccd884280e27e229e5f96d77efc4c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `openjdk:11-jdk-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull openjdk@sha256:eb6aae9f9e4364110893e7c391f78771410dfd51e1c8be501e2fc79ccda7f332
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2465601948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71dc6ec825ba4f22255560dd53b6d94fc2c61d24d5773c72d3d766425ac32275`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Apr 2020 21:51:51 GMT
ENV JAVA_HOME=C:\openjdk-11
# Tue, 14 Apr 2020 21:52:30 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 14 Apr 2020 21:52:31 GMT
ENV JAVA_VERSION=11.0.6
# Tue, 14 Apr 2020 21:52:32 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_
# Tue, 14 Apr 2020 21:52:33 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Tue, 14 Apr 2020 21:54:04 GMT
RUN $url = ('{0}x64_windows_{1}.zip' -f $env:JAVA_BASE_URL, $env:JAVA_URL_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 14 Apr 2020 21:54:06 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76226cfc56487958b0dd09e402ad764ebe45c0d60a9f371b313f464139d53067`  
		Last Modified: Tue, 14 Apr 2020 22:20:19 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0881d2c023f862a62321635e36b1908f2cd044ddf41621a6b369b072550b481f`  
		Last Modified: Tue, 14 Apr 2020 22:20:20 GMT  
		Size: 4.7 MB (4669064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e86499b57031135e5dfbb0a88b2f7302eef891a37c5a6da306a74338a2b7d64`  
		Last Modified: Tue, 14 Apr 2020 22:20:16 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad470e12a91d3a00aa6fbe218e6586e918db440dd9e621d76154d0e35e237f3`  
		Last Modified: Tue, 14 Apr 2020 22:20:16 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e43e1c318bf1153a2f61e3794d0fd086f5873f30330a3dd3921cb38ca25d91b`  
		Last Modified: Tue, 14 Apr 2020 22:20:16 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f296a4fb5aad214669b31241f376bbda7087962b61cbcb48ed3c0e99be7895a6`  
		Last Modified: Tue, 14 Apr 2020 22:21:04 GMT  
		Size: 190.2 MB (190218873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fd3b96fcf41e57de21381d617daa07239b114e03b5f1b79b243ace289bf017`  
		Last Modified: Tue, 14 Apr 2020 22:20:16 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
