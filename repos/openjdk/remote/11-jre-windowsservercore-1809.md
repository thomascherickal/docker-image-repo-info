## `openjdk:11-jre-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:f2c44ef353f20752d1e1049f5e617a4600e043e764430d13c658fb2ddf43872d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `openjdk:11-jre-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull openjdk@sha256:261484629bd7cef73dffa0a61443a102112287f59239d9c4626b112deb7772f3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2404206829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5152a349a74c6b45c2800324d920b03b76df213289b9f6ee277508d8e738658`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Sep 2020 21:01:49 GMT
ENV JAVA_HOME=C:\openjdk-11
# Tue, 08 Sep 2020 21:02:34 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 08 Sep 2020 21:02:34 GMT
ENV JAVA_VERSION=11.0.8
# Tue, 08 Sep 2020 21:10:10 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_x64_windows_11.0.8_10.zip
# Tue, 08 Sep 2020 21:11:01 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
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
	-	`sha256:2d87797081953a2dd634c8dbcf1364ab6f93014d27e8473e2ac2aa9bd74a4799`  
		Last Modified: Tue, 08 Sep 2020 22:37:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf49d2b57e1cbf7258bc67c9119cbcfe8782987a001a2e16657ba8b66e8ffbfb`  
		Last Modified: Tue, 08 Sep 2020 22:37:33 GMT  
		Size: 9.1 MB (9129272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5ca8ab95ab9df34a105e01d9d86bbb474a28195b9fa4994f736bee721de802`  
		Last Modified: Tue, 08 Sep 2020 22:37:30 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49d71b8ffd35bacd9299d7f9b622c5e31a40cf5dd3a615d2b2296b4b04de9dc`  
		Last Modified: Tue, 08 Sep 2020 22:40:00 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d86b3cc104e1dad89ee19a90a071689b0d2e31e7db4b02006468352f0584092`  
		Last Modified: Tue, 08 Sep 2020 22:40:09 GMT  
		Size: 43.8 MB (43800789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
