## `openjdk:17-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:7a31ff7a8716f8b23370c6126900feda25b6db4e1836785a5a78451f0b944203
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `openjdk:17-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull openjdk@sha256:4f61685d203d6bbdaf348d0f2576c014b3f52ccc98bf061bd7c9c37fc56be12e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2586409719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:647d17f67b96e7fd8c408e7d454ee0ca24219268ea91932943e1dc2cafe80e04`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 18:50:31 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Mon, 28 Dec 2020 21:15:10 GMT
ENV JAVA_HOME=C:\openjdk-17
# Mon, 28 Dec 2020 21:45:49 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Mon, 28 Dec 2020 21:45:50 GMT
ENV JAVA_VERSION=17-ea+3
# Mon, 28 Dec 2020 21:45:51 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/3/GPL/openjdk-17-ea+3_windows-x64_bin.zip
# Mon, 28 Dec 2020 21:45:51 GMT
ENV JAVA_SHA256=6208dba1b22a0c2cbe91bf4073bf19b551c402667b71bbaa4f91ab0445b89e5a
# Mon, 28 Dec 2020 21:47:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 28 Dec 2020 21:47:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935e3005fe76a11e222d9322d452d314edc4ba767499cc7c7e9f7cff154513fc`  
		Last Modified: Wed, 09 Dec 2020 19:32:28 GMT  
		Size: 9.2 MB (9236222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035937c4c9eb2ad6c44e21bdb49ff2b2b54991c36e355984bb4a4f7771ba5b83`  
		Last Modified: Mon, 28 Dec 2020 21:58:04 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e6b3e04cd5a526f1b0b797d7fc36cd423522dcf46912d2ce7f5f38593c3413`  
		Last Modified: Mon, 28 Dec 2020 21:58:06 GMT  
		Size: 325.5 KB (325501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120d8d735b22965b3d649b77cb389716730804a94846b1e7dfd1670c9ed8aeda`  
		Last Modified: Mon, 28 Dec 2020 21:58:01 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b7ad2a20459959290bf85e3b8e85c9c8c7077692da84082b424174a643fe93`  
		Last Modified: Mon, 28 Dec 2020 21:58:01 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f56555d7a7eb77b44c93a5f940f8fbcafe41dd28f3f7d6d0f988bb785fc921`  
		Last Modified: Mon, 28 Dec 2020 21:58:01 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbeb92adb174ef5452518c015b37e81a2f855748dd20eea22388520c63d00289`  
		Last Modified: Mon, 28 Dec 2020 22:01:29 GMT  
		Size: 186.0 MB (185966734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e8dcc7484e0a9907496d135c6b54bc65a13571f7685e5d24b51410bf37715a`  
		Last Modified: Mon, 28 Dec 2020 21:58:01 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
