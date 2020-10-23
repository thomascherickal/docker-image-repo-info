## `openjdk:11-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:0743fbfff8a3a75c99c7673bd7266b24af3623e2b9fffa22e213ee14f16c583c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `openjdk:11-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull openjdk@sha256:5e1b8d09d42370ad0332ee75267213b0136c810baad2ace82271b8b20232394a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5951815764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3639e992bac910b32980a83ce4c2d7f191156986fe8b8e09a4fa88d819cb8c7f`
-	Default Command: `["jshell"]`
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
# Thu, 22 Oct 2020 23:23:29 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9%2B11/OpenJDK11U-jdk_x64_windows_11.0.9_11.zip
# Thu, 22 Oct 2020 23:25:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 22 Oct 2020 23:25:54 GMT
CMD ["jshell"]
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
	-	`sha256:80814cc00da64195d934c9b5141c4d076d0778f720199efe361b2aeac2827bf1`  
		Last Modified: Thu, 22 Oct 2020 23:37:01 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32768cfd57c8c47d9a791b01956c6439476a359d7682dff5ed43e8255418246a`  
		Last Modified: Thu, 22 Oct 2020 23:37:33 GMT  
		Size: 200.5 MB (200536865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca51e8237cf49bb790581078518b1975875a5eb63c8ed64d34241d69754e22d`  
		Last Modified: Thu, 22 Oct 2020 23:37:01 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
