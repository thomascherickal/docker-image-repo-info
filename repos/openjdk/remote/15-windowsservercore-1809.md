## `openjdk:15-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:6cfeb20f9e5e038be141cdf279eea51cf47dd28e19f4151ee63ba57f53370e75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `openjdk:15-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull openjdk@sha256:a3cd688e0d3140c309684262e8d2f69de1a4ee82cb1f5c05ff0d98078d53b2d4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556734485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a74bee14e724da52db6551e393e8970a818e6e9afd582134043b2856dbf96f2f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Sep 2020 20:05:13 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Tue, 08 Sep 2020 20:15:04 GMT
ENV JAVA_HOME=C:\openjdk-15
# Tue, 08 Sep 2020 20:15:29 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 08 Sep 2020 20:15:30 GMT
ENV JAVA_VERSION=15
# Tue, 08 Sep 2020 20:15:30 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_windows-x64_bin.zip
# Tue, 08 Sep 2020 20:15:31 GMT
ENV JAVA_SHA256=764e39a71252a9791118a31ae56a4247c049463bda5eb72497122ec50b1d07f8
# Tue, 08 Sep 2020 20:17:20 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 08 Sep 2020 20:17:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b301c9d4a0d508778c4b1506920d1304eb5d8c3d5a73ee0a1b522db1e8b9d70`  
		Last Modified: Tue, 08 Sep 2020 22:27:29 GMT  
		Size: 9.1 MB (9130218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b841ce0b0858984d74f0e6b7f4473287fe725dc9fd492bc26867d0044b03e9ed`  
		Last Modified: Tue, 08 Sep 2020 22:29:41 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899b1f7cf8f44bf2efa050b83e9d1d8f53137b9999f9558e1c1ffede6351ab79`  
		Last Modified: Tue, 08 Sep 2020 22:29:42 GMT  
		Size: 295.6 KB (295589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98af0bbd93dcef818aac5ec679ab81624818c052a52c8f3c723c71aca06751b1`  
		Last Modified: Tue, 08 Sep 2020 22:29:39 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af800bfb23fe2336b1a33f3129820c22932812968fbc371a2d70f17eda4fc6a`  
		Last Modified: Tue, 08 Sep 2020 22:29:39 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f238c2338962a477b98a2d24a075c47ac3593bdce392259962586c9fd54962`  
		Last Modified: Tue, 08 Sep 2020 22:29:39 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409b41098c8357d921f73bf0350904e4c85ef3af7eb5436342f20677ecffc3d4`  
		Last Modified: Tue, 08 Sep 2020 22:30:00 GMT  
		Size: 196.0 MB (196029594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d7725fcf0f22521417499b84f1a3b867f396fb3c13cfad98513a91edd878e3`  
		Last Modified: Tue, 08 Sep 2020 22:29:39 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
