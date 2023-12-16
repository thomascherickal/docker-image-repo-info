## `openjdk:23-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:ba55dd9a9737de30df0465f3d6e79a973de50164de913973b3aef0360e40f951
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `openjdk:23-jdk-windowsservercore-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull openjdk@sha256:b830cf78dde50071a036884bb94fd1bb6175409e16fc577746ef7db7290fa6ff
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2258285936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b93826679e943e960222935631add0dfdb52410c102e897ac4e8a1bfe0e29ac`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 04 Dec 2023 11:24:49 GMT
RUN Install update 10.0.17763.5206
# Fri, 15 Dec 2023 22:20:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 15 Dec 2023 22:21:15 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:21:16 GMT
ENV JAVA_HOME=C:\openjdk-23
# Fri, 15 Dec 2023 22:21:36 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:21:36 GMT
ENV JAVA_VERSION=23-ea+1
# Fri, 15 Dec 2023 22:21:37 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk23/1/GPL/openjdk-23-ea+1_windows-x64_bin.zip
# Fri, 15 Dec 2023 22:21:37 GMT
ENV JAVA_SHA256=b60d20ad423ec31c88a18679854a31bdef66003224227d86dcbd10781fe14db1
# Fri, 15 Dec 2023 22:22:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 15 Dec 2023 22:22:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ae5ad761bfd7e5fb48c234de8722eaa28e17e2c956816fecb417ab6259c29`  
		Last Modified: Tue, 12 Dec 2023 19:14:24 GMT  
		Size: 409.1 MB (409088642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b07be79186bada004046f6b749cb6555157f896380e88635714586b3b96e3a`  
		Last Modified: Fri, 15 Dec 2023 22:22:20 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d96aca320c72c08112922be54c59d0cdeeadfb127ce8e0a7befd5f3976db09`  
		Last Modified: Fri, 15 Dec 2023 22:22:20 GMT  
		Size: 485.4 KB (485386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38467a9a9f8a64bf926ea81cd7db78dfcfe07d24eb3d890adc15a843cf6cef2b`  
		Last Modified: Fri, 15 Dec 2023 22:22:20 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af5242e82081edaa4b479eeffdd04a62c5c42ee16c08b31d1804e31f1eb4d68`  
		Last Modified: Fri, 15 Dec 2023 22:22:20 GMT  
		Size: 330.0 KB (329963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d27aa5f28e6d90fc737293538f8746708be4133598f7af304e23e09b85c15f`  
		Last Modified: Fri, 15 Dec 2023 22:22:19 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24c73731f85bc23cd10201ba4a9c8e37f3c2605ef556c3f9ca83b28c7293e3d`  
		Last Modified: Fri, 15 Dec 2023 22:22:19 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edadf6896caeb6df946fc3e6e77c18e3ee3fbaf9897d47eff04eab5186cfadc4`  
		Last Modified: Fri, 15 Dec 2023 22:22:19 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd87cc9c84e32ecd1b704df4fca63235b4a12662884bee2ed49eb20ee04c028`  
		Last Modified: Fri, 15 Dec 2023 22:22:31 GMT  
		Size: 197.8 MB (197753833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714de47a6a6f9b79b48c738744597137bee13da27ed4a8721186e926c1f150dc`  
		Last Modified: Fri, 15 Dec 2023 22:22:19 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
