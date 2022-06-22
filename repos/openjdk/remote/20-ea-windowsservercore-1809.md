## `openjdk:20-ea-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:04ec23de658850cae4eacb3450a0f9fd5b72f3fbaab3437a1c2d47ebefad678a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `openjdk:20-ea-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull openjdk@sha256:31ef4b0e5e2d74692190368bfde0bd3481d2c228e81d7a66a6887cacf547071c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2856495708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:225dd3ba6e1bdd06ee63bd0a67763c99bfdea6dbe678e5809ea43d6731a9c609`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 19:33:08 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Jun 2022 01:16:22 GMT
ENV JAVA_HOME=C:\openjdk-20
# Thu, 16 Jun 2022 01:17:35 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 22 Jun 2022 00:45:03 GMT
ENV JAVA_VERSION=20-ea+2
# Wed, 22 Jun 2022 00:45:04 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/2/GPL/openjdk-20-ea+2_windows-x64_bin.zip
# Wed, 22 Jun 2022 00:45:05 GMT
ENV JAVA_SHA256=8dc5a274cd002d32ae4c8f6561afb4b620763ac5c05a3fdf77ea1b5ad58fbe3a
# Wed, 22 Jun 2022 00:46:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 22 Jun 2022 00:46:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75415e053743ebceabbf30d0a8101d97dd712c88fc012c45f1df824cbac48e21`  
		Last Modified: Wed, 15 Jun 2022 20:05:58 GMT  
		Size: 354.4 KB (354400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52024d1a50366ffd4635321735cd38ce0ecab43a1ba938284d4286b6020140ef`  
		Last Modified: Thu, 16 Jun 2022 01:29:40 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4732abfe811150ac2b9a2ccb0f838bf2f402b7f56952056d2f28ba681fc8b120`  
		Last Modified: Thu, 16 Jun 2022 01:29:40 GMT  
		Size: 312.4 KB (312396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b424ef6bf361dc694b75aafe2f3eaa695fa11e4fba0bbdf2b941b7483a11bab`  
		Last Modified: Wed, 22 Jun 2022 02:24:52 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ede2556a664b15c0cef8a75604b73e8fb578b36f61b3fb43da1642ce98202c`  
		Last Modified: Wed, 22 Jun 2022 02:24:51 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af19c85b4f898b8502a48295502da644610bdf94283ffbde478b4f01e6771c5a`  
		Last Modified: Wed, 22 Jun 2022 02:24:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f921f8c87da9c5303348563fd479c99fa87f45c9be9ea5e40ee4f86e977f66b`  
		Last Modified: Wed, 22 Jun 2022 02:28:24 GMT  
		Size: 192.5 MB (192540612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e58c00fc9ecebbd50398b5268ff465ec4f068bd8cd40d99733b2cdd81e8e832`  
		Last Modified: Wed, 22 Jun 2022 02:24:52 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
