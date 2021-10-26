## `openjdk:18-jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:e435c9349c0a0e508eaa576768c3cb612844580313b1dfc631b5a461e531874a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.288; amd64

### `openjdk:18-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.288; amd64

```console
$ docker pull openjdk@sha256:5cf6a20df8fc357aa3e3a197e32f414e14052b8545cd66ae82fba05f5a1a1bb8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2326482009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fedb9ab7564e05999cfa7da7f218a729679a4947b313c960b65aec87e5a8c8c1`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 07 Oct 2021 11:33:56 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Oct 2021 12:26:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 25 Oct 2021 23:16:39 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Mon, 25 Oct 2021 23:16:40 GMT
ENV JAVA_HOME=C:\openjdk-18
# Mon, 25 Oct 2021 23:17:02 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 25 Oct 2021 23:17:03 GMT
ENV JAVA_VERSION=18-ea+20
# Mon, 25 Oct 2021 23:17:04 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_windows-x64_bin.zip
# Mon, 25 Oct 2021 23:17:05 GMT
ENV JAVA_SHA256=9a0adb8304f31d0e05a1d4a2d848e989e8c195027ef954afdb789977285287e8
# Mon, 25 Oct 2021 23:18:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 25 Oct 2021 23:18:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b03bbc71f9254a4ad2fba472595c859655b9d0cfefa638928416e277e0f0d497`  
		Size: 889.8 MB (889767519 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b201e45e5b11128e36517715f5b6ae98e5782737c1b112a5fae2aa83206f57bf`  
		Last Modified: Wed, 13 Oct 2021 13:23:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a947ce19e17c924828c9323a0de0ab956cabefde1b9245295f097feaff9f13a`  
		Last Modified: Tue, 26 Oct 2021 01:22:57 GMT  
		Size: 628.9 KB (628862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df973053814857f61afa97656cc85bcc253c39d40edf7971e695893f5a006d6f`  
		Last Modified: Tue, 26 Oct 2021 01:22:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229e005f3546fff3d9eea6854af9a4671d474eadd333aca8dbebbed48efed762`  
		Last Modified: Tue, 26 Oct 2021 01:22:57 GMT  
		Size: 560.1 KB (560056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c23c0297f537b1f89b8c35c1c6d7b8250ec29a7f5c3cfc2c4a200131576bffd`  
		Last Modified: Tue, 26 Oct 2021 01:22:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e8d074252552e2ef542b88fd04b80a4d1cb756c7dc005fae016c2af9f31d32`  
		Last Modified: Tue, 26 Oct 2021 01:22:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78a2ca7bff267054e62f2a2609a3ac5e23e46f0c5cf41b30cf6d15a99f6963f`  
		Last Modified: Tue, 26 Oct 2021 01:22:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737d8b552acee8df9017805be2f2a31883234ea2eab7049cec9b4b0bc469d9d5`  
		Last Modified: Tue, 26 Oct 2021 01:26:16 GMT  
		Size: 183.8 MB (183818024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f444d2a5fd388d24f6539cae11b3ae18637a2468f1543e95ac1d822cf983808`  
		Last Modified: Tue, 26 Oct 2021 01:22:54 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
