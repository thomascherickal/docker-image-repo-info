## `openjdk:17-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:c8a139b24e6a7eec77017b916774982d4b4a814d3ae3d2b9f797e533188565d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `openjdk:17-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull openjdk@sha256:c0255f4dbe5c02859431bcd8dc5a92a0e09b264dce19c0df057f720966e6292f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2656510566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd4a92862cc9813120998f27fe9d357405885764d38632ec0213449f0e38a7a8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 16:45:00 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Apr 2021 16:45:01 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 14 Apr 2021 16:45:32 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 10 May 2021 23:27:23 GMT
ENV JAVA_VERSION=17-ea+21
# Mon, 10 May 2021 23:27:24 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/21/GPL/openjdk-17-ea+21_windows-x64_bin.zip
# Mon, 10 May 2021 23:27:26 GMT
ENV JAVA_SHA256=17d3a7b8b2fbbeea19ac5df7788db20a09642bdee3116b89ad91690d95717313
# Mon, 10 May 2021 23:28:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 10 May 2021 23:28:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3d005d273e9763b53b5f1034b1284bcce913f8dbd1855d70f561efc09be849`  
		Last Modified: Wed, 14 Apr 2021 17:36:21 GMT  
		Size: 5.1 MB (5074608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ab40deb7e8f2f68f8ddebdcf9a4ccf7112615246fd6c75d400cd491cdac535`  
		Last Modified: Wed, 14 Apr 2021 17:36:20 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3fa76ecf2e81ab47fe24f1aeab9427a58be444cc60cf90038197c769d046a0`  
		Last Modified: Wed, 14 Apr 2021 17:36:21 GMT  
		Size: 319.5 KB (319514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89916bc444890355a29b1aff3f44326f14ef259baf40909901264140374fcf86`  
		Last Modified: Mon, 10 May 2021 23:39:46 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4baa075f65f4d7043a4a90f1b588f66e59db550afcf869ec9061fc2f13a40c7a`  
		Last Modified: Mon, 10 May 2021 23:39:46 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797b088dfc545b60d101e9632451e67e737ce545a555087008f07155935a239c`  
		Last Modified: Mon, 10 May 2021 23:39:46 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73d230de2f6f49c4884e2d172d5caf00a57dc640e919e2bb37356fbbe91fadd`  
		Last Modified: Mon, 10 May 2021 23:40:08 GMT  
		Size: 181.4 MB (181354038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9aa950f825ed94bb6c33b1c9d3d269d77d1c9bdc629d49359ee3b0d5f86d89`  
		Last Modified: Mon, 10 May 2021 23:39:46 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
