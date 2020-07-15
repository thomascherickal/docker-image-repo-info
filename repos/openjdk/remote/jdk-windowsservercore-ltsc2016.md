## `openjdk:jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:ab54ce210bcd6c40fa83c39fa22bc257c377f99faa67b640f640b3f0b1a88001
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64

### `openjdk:jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.3808; amd64

```console
$ docker pull openjdk@sha256:1058f45e5bdb125c7689db76e1af5a65589d82466dd250f1b3a8641e7b836d9f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5956447097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c60c3804546d532ae302d06c441059ab5dfda00afe300618f8e4ca3434b895`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 01:50:16 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 15 Jul 2020 02:07:56 GMT
ENV JAVA_HOME=C:\openjdk-14
# Wed, 15 Jul 2020 02:09:20 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 15 Jul 2020 02:09:21 GMT
ENV JAVA_VERSION=14.0.2
# Wed, 15 Jul 2020 02:09:22 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk14.0.2/205943a0976c4ed48cb16f1043c5c647/12/GPL/openjdk-14.0.2_windows-x64_bin.zip
# Wed, 15 Jul 2020 02:09:23 GMT
ENV JAVA_SHA256=20600c0bda9d1db9d20dbe1ab656a5f9175ffb990ef3df6af5d994673e4d8ff9
# Wed, 15 Jul 2020 02:12:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 02:12:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccabcd61311861039196ce34ec8b8b74f236a3b135a888ca230811c6f8a439bc`  
		Last Modified: Wed, 15 Jul 2020 02:43:13 GMT  
		Size: 9.9 MB (9852381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73580861f0a38e97a8591c4a4a2e32a0255cb5ff50b9841e1d903b25f2dfc8ee`  
		Last Modified: Wed, 15 Jul 2020 02:47:56 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091c1af47add49d684a946f7ff6f59f1c9941f1556c7ef7f1a17f3b7c16d439c`  
		Last Modified: Wed, 15 Jul 2020 02:47:57 GMT  
		Size: 5.3 MB (5331610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c25bc3d312eb6035c9f8b50188f7f4c7f53113e67fe31c6c77eb40fd73a4238`  
		Last Modified: Wed, 15 Jul 2020 02:47:53 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe2b1a61c035b4c8bdcfbee31511be45f0ddab9f903133cf24c2ed264082e7b`  
		Last Modified: Wed, 15 Jul 2020 02:47:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0e077cf4a65602a5457227a672d1977e9cb5d4619d406b185683161dcc64ff`  
		Last Modified: Wed, 15 Jul 2020 02:47:53 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cc37a18e6e969c8cf7556d32e0224485a5ec3fb372124c7b9db74a01211720`  
		Last Modified: Wed, 15 Jul 2020 02:48:16 GMT  
		Size: 203.8 MB (203794211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbb1b9260d697cb9cc8ad43f2ce459b9ca92ebdcd2438976ab45b2afd52fb8f`  
		Last Modified: Wed, 15 Jul 2020 02:47:53 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
