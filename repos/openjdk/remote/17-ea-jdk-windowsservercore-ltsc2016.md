## `openjdk:17-ea-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:c5d0116fae787230b7a834a3c88bfe65a50dabb26de18ea66236819fe355a38b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `openjdk:17-ea-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull openjdk@sha256:ffbbafd68b6fa1ef52912e81a9dfd9bf9f00807e154afc5efa9e6d1823e9f834
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5997233218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ab1723df17c5783eb3c67d718669663708156e232f4368bb9b486da91b99d68`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 16:48:32 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Apr 2021 16:48:33 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 14 Apr 2021 16:50:24 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 10 May 2021 23:28:55 GMT
ENV JAVA_VERSION=17-ea+21
# Mon, 10 May 2021 23:28:57 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/21/GPL/openjdk-17-ea+21_windows-x64_bin.zip
# Mon, 10 May 2021 23:28:58 GMT
ENV JAVA_SHA256=17d3a7b8b2fbbeea19ac5df7788db20a09642bdee3116b89ad91690d95717313
# Mon, 10 May 2021 23:31:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 10 May 2021 23:31:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e39566a6e39d3a16eac2642132dd97b58680502417c33529cb3b20734e62ffd`  
		Last Modified: Wed, 14 Apr 2021 17:37:12 GMT  
		Size: 5.6 MB (5648642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501b89977f05abcd65cccdbfec96af4495b33ee4acc7932a4bf2a77874b2d40`  
		Last Modified: Wed, 14 Apr 2021 17:37:09 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e79ef171c9bf6c1503c79940d0393f3121096ad7a3a91bc2d65c511c78175e8`  
		Last Modified: Wed, 14 Apr 2021 17:37:11 GMT  
		Size: 5.6 MB (5595448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6847ed99c59ef7e1e71559c8446e178137af8ce74cbaec00e0b4cea755800703`  
		Last Modified: Mon, 10 May 2021 23:40:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9805d82bbf8ef434f6dc3a10a0235fa2740ff153c7bca89f06e81e03df596d9b`  
		Last Modified: Mon, 10 May 2021 23:40:36 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced3ae82e635abd41d37d1f3357c3fcf11fb4d0053b81588eacc04b8a975827`  
		Last Modified: Mon, 10 May 2021 23:40:36 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb9dbc7719886472a9a0f2c310edd6c727352ecd83660cade5b35ec74f4f6c6`  
		Last Modified: Mon, 10 May 2021 23:41:01 GMT  
		Size: 191.1 MB (191096751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0358b8597af426292efc8e2250b9cf9886d4b0f452d07f0757e70e9073be7c3d`  
		Last Modified: Mon, 10 May 2021 23:40:36 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
