## `openjdk:19-ea-34-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:c65df8a0eb4f5d097dae75e6593c175d98ad2652a1db9553bd044a9da1b25da7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `openjdk:19-ea-34-jdk-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull openjdk@sha256:73d9b156343f2c4adafbc2f58f49bc454bc8cbaf7f4b3c1e36e4fe0432dd4a5c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2864273313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a3cf72be7f0a7917c3d1fcb57599ca7a34a4b9bf3b25eea4081b2df416043f9`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jul 2022 15:50:04 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Jul 2022 15:55:10 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 13 Jul 2022 15:56:04 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 08 Aug 2022 22:20:28 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 22:20:29 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_windows-x64_bin.zip
# Mon, 08 Aug 2022 22:20:30 GMT
ENV JAVA_SHA256=5d3ac1a89d92a142588bc8546aa737c37d1971bcff17810b5ff947790c97e623
# Mon, 08 Aug 2022 22:21:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 08 Aug 2022 22:21:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acf5949ddc551d281d19646d7dbeb4f3772073cf86c194f6d98c8afe422f3b5`  
		Last Modified: Mon, 18 Jul 2022 21:21:50 GMT  
		Size: 353.5 KB (353532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ef755dcec989c5860b62157e6a71a3161b651df08ebc5d41a441c82db2bda3`  
		Last Modified: Mon, 18 Jul 2022 21:23:59 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be3865968b6d273d0d991753302d14841ef7355875ec01f046c8f653d019223`  
		Last Modified: Mon, 18 Jul 2022 21:23:59 GMT  
		Size: 311.7 KB (311730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada3e77ee115d05d9a9899adedac83218670e2975f4f7f84e328cfc9f8b4c622`  
		Last Modified: Mon, 08 Aug 2022 22:30:18 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2f0ce27c6e3be4355cd0ba7da5234dadcfa3b950d8d7128e1066102cf18714`  
		Last Modified: Mon, 08 Aug 2022 22:30:18 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e956b3127157cf40c5e0e9e65697d20701f0de8f7f78a9357499077a605503`  
		Last Modified: Mon, 08 Aug 2022 22:30:18 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3567d27f19e2c439737bfc0987e27b26934646f84f746995db345a95988f5f4f`  
		Last Modified: Mon, 08 Aug 2022 22:30:38 GMT  
		Size: 191.6 MB (191555768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbce2153197de2622aca1bcc9eff846120d07cd5d2015c0e4e5a227135f69d2`  
		Last Modified: Mon, 08 Aug 2022 22:30:18 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
