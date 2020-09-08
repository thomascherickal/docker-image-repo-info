## `openjdk:8-jre-windowsservercore`

```console
$ docker pull openjdk@sha256:7b6a832871af072f7d3264d84ae3913c09892ccbd3f6289502e57fd10d32f22b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `openjdk:8-jre-windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull openjdk@sha256:6232b47411d75787e4fba876591c1f114eb9cceb0cfc44d3f435911556201528
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2402498895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eaa4c6b8f6d4fb8d44504225d4d700609c577ec15654114730bdaf243dbb37e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Sep 2020 21:13:52 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 08 Sep 2020 21:14:32 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 08 Sep 2020 21:14:33 GMT
ENV JAVA_VERSION=8u265
# Tue, 08 Sep 2020 21:20:49 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_windows_8u265b01.zip
# Tue, 08 Sep 2020 22:22:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c150df4792583673411faa35e279fb99bceda9714a46fbdf52806587358f9b`  
		Last Modified: Tue, 08 Sep 2020 22:42:39 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f43679dd834d5e7af97980fee2dd8700bc6553fd4d8a3eaf993db73fe422bd`  
		Last Modified: Tue, 08 Sep 2020 22:42:42 GMT  
		Size: 9.1 MB (9129525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301e537a5004d9951fcfb780370a05bf13dd2eb9e8471564e4f216aa0452f8c4`  
		Last Modified: Tue, 08 Sep 2020 22:42:38 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dc61ed1fd2a013e63ce8092bc1458644aa22568c1f47c47bdac709f47a59e0`  
		Last Modified: Tue, 08 Sep 2020 22:44:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0b9d88349969a3e42d320c1535cda7d09a91790b0ff3e3a0999e735c972f64`  
		Last Modified: Tue, 08 Sep 2020 22:44:46 GMT  
		Size: 42.1 MB (42092566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8-jre-windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull openjdk@sha256:41aefd23ef94a79df24c0d534d80eefd3c1fbc4f3810f3c2211dffb2e2736fe1
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5796418122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b90180fff500b10c777cd1eb18c42921cb0ef7b90f19d5df9e4614fbed2970d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Sep 2020 21:16:03 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 08 Sep 2020 21:17:28 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 08 Sep 2020 21:17:29 GMT
ENV JAVA_VERSION=8u265
# Tue, 08 Sep 2020 22:22:22 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_windows_8u265b01.zip
# Tue, 08 Sep 2020 22:24:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3358b74428811280b1f3dda3449fde85aa183b9ab00c8c2544314f6dd6f95c6`  
		Last Modified: Tue, 08 Sep 2020 22:43:08 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe579e67c19d6eb6c16d0505037dd4c354bebc669d4f7fcbc665850b5fe93bc3`  
		Last Modified: Tue, 08 Sep 2020 22:43:11 GMT  
		Size: 9.9 MB (9880038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60f0fbc101f430aae5765a2b407a78cb246f06456704a6e7e8c57ffa637ec1e`  
		Last Modified: Tue, 08 Sep 2020 22:43:08 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3adf35584a979b1cba73551eb3b61b6880f5678441b89a86e09ba1c4ef4a46`  
		Last Modified: Tue, 08 Sep 2020 22:44:56 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a65be0af409fb72d154f34584a70ab72a4e705ff5ce3cefbb72845f1e6d2611`  
		Last Modified: Tue, 08 Sep 2020 22:45:04 GMT  
		Size: 47.3 MB (47279136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
