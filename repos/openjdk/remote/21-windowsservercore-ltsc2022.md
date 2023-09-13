## `openjdk:21-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:ad814fb8fb955e4f8ac1740b2e444e709b48b01b39aff4d5be11c53bac532d20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `openjdk:21-windowsservercore-ltsc2022` - windows version 10.0.20348.1970; amd64

```console
$ docker pull openjdk@sha256:1d0cb8f938a2c9120b30dbfb4f0c909a8c2ccc443eb54bb1aa2b7f437aca7d01
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2036348001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:124df0d460b86810e9678be525a970be45824a1eed4284d5dc3d350c881249dc`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 01 Sep 2023 00:43:48 GMT
RUN Install update 10.0.20348.1970
# Wed, 13 Sep 2023 01:35:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Sep 2023 05:14:15 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Sep 2023 05:19:56 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 13 Sep 2023 05:20:18 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 13 Sep 2023 05:20:19 GMT
ENV JAVA_VERSION=21
# Wed, 13 Sep 2023 05:20:20 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_windows-x64_bin.zip
# Wed, 13 Sep 2023 05:20:20 GMT
ENV JAVA_SHA256=5434faaf029e66e7ce6e75770ca384de476750984a7d2881ef7686894c4b4944
# Wed, 13 Sep 2023 05:21:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 13 Sep 2023 05:21:10 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca8e06011ab171ad74cda49c7c305e791965aef283d5b7c2b987dd5388e6c7`  
		Last Modified: Tue, 12 Sep 2023 18:24:42 GMT  
		Size: 448.7 MB (448675362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f40969dbf1e035a6c49e7c40b216960e3ee98ec3b76f76f9fe4498d0110bee`  
		Last Modified: Wed, 13 Sep 2023 02:15:22 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b411249ef1c74d6763984f0b9b085ac311c6e49aba35a7dbbc1d42264a11ba`  
		Last Modified: Wed, 13 Sep 2023 05:25:31 GMT  
		Size: 462.9 KB (462878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356cafbb83690378d2b5321a71a7676f0d3cdaa85c78464207e8bd68a728044a`  
		Last Modified: Wed, 13 Sep 2023 05:27:24 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65146080cde20c7b199f9bcc2ba70ee2006d78ead09713738847471584889e46`  
		Last Modified: Wed, 13 Sep 2023 05:27:24 GMT  
		Size: 275.1 KB (275088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6844f3e5f864d71ff5b15b4d10e849352bbe5753b8389ec7722540c53d28202`  
		Last Modified: Wed, 13 Sep 2023 05:27:22 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42ea48777c2f1c5acb081744a1441d3bf58004682e34ca65d8b665e7cd86c2`  
		Last Modified: Wed, 13 Sep 2023 05:27:22 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96d1dd7c327a05e2dc1b8091c70d6f4ee6c1984c121415822d8a45d9af820de`  
		Last Modified: Wed, 13 Sep 2023 05:27:22 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bfd1ee811e4bdef25ffa1ffe97e6c8dd625b022bc00d1a36d2109ffefad6b5`  
		Last Modified: Wed, 13 Sep 2023 05:27:41 GMT  
		Size: 198.3 MB (198327510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f57a7cab1c78f3e9f5de3a8f030b2eed357fe4e749f858394af63adf03b0adf`  
		Last Modified: Wed, 13 Sep 2023 05:27:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
