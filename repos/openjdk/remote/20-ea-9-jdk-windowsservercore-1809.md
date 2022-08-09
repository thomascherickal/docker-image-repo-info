## `openjdk:20-ea-9-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:89d217b4201c36e88c64049227b11d18a6baa469de2086d7de24f0c2d812a066
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `openjdk:20-ea-9-jdk-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull openjdk@sha256:788a76b6c4df075c483abe3cecb0a74e614e47ae9e3261e78d2cf50e1caaa45b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2865411640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6fee9c2e8361661b75762073ba53e31b92d299bb5c16e5df707ed813f6ed351`
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
# Wed, 13 Jul 2022 15:50:05 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 13 Jul 2022 15:50:57 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 08 Aug 2022 22:16:20 GMT
ENV JAVA_VERSION=20-ea+9
# Mon, 08 Aug 2022 22:16:21 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/9/GPL/openjdk-20-ea+9_windows-x64_bin.zip
# Mon, 08 Aug 2022 22:16:22 GMT
ENV JAVA_SHA256=69540c9291f1d68616035ff98d95ec4b0bc9fe19d1bddbc4fe091a8c70fcf4f0
# Mon, 08 Aug 2022 22:18:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 08 Aug 2022 22:18:12 GMT
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
	-	`sha256:78ca4f44b32042d608ce9b62563bbff47ca623a4ca4ca22575a680b990a1d675`  
		Last Modified: Mon, 18 Jul 2022 21:21:50 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4525c6bc4913f609856004e14ff912919aa9219c0df562367a0764e7ae034f5`  
		Last Modified: Mon, 18 Jul 2022 21:21:50 GMT  
		Size: 311.6 KB (311646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40297aa2a28046c1af166e101764d184f075dcbbe4f9c4551b2d41f4922850e0`  
		Last Modified: Mon, 08 Aug 2022 22:28:09 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8e73ad06f9f86ff7f07414d86afb04cd01dde9184a416f1cbd3c340d192333`  
		Last Modified: Mon, 08 Aug 2022 22:28:09 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb10514123500d3bf1736a5cc80edab36dcdbf03968531bc6b61fd7890ed9406`  
		Last Modified: Mon, 08 Aug 2022 22:28:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86016574b39d5cc159d28909edf97563d58c65253299a5085ad9c1bc7642883b`  
		Last Modified: Mon, 08 Aug 2022 22:28:32 GMT  
		Size: 192.7 MB (192694213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d2e200b39934b01dde65acf39cdca1cc157d1ce4edf73d659d09347eff3bb8`  
		Last Modified: Mon, 08 Aug 2022 22:28:09 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
