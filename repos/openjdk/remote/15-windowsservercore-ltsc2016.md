## `openjdk:15-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:35c0166c20c3005e81b1d838b8617d9c7ea8ea2c2415bd22951d9da45fc09c47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `openjdk:15-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull openjdk@sha256:7b987f2ddd1c1b070e8498228046a3803e759675816a1e1964bba7403518ff97
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5955700284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20de6c05656b346851b8b8139936f071dc65d602c911c0061517a879df1340e2`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Sep 2020 20:09:21 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Tue, 08 Sep 2020 20:17:30 GMT
ENV JAVA_HOME=C:\openjdk-15
# Tue, 08 Sep 2020 20:18:48 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 08 Sep 2020 20:18:49 GMT
ENV JAVA_VERSION=15
# Tue, 08 Sep 2020 20:18:50 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_windows-x64_bin.zip
# Tue, 08 Sep 2020 20:18:51 GMT
ENV JAVA_SHA256=764e39a71252a9791118a31ae56a4247c049463bda5eb72497122ec50b1d07f8
# Tue, 08 Sep 2020 20:21:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 08 Sep 2020 20:21:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbeff382f1371b6819ca1ae810348afda32084cbd4526c4114c9ff5f85a5d6d`  
		Last Modified: Tue, 08 Sep 2020 22:28:21 GMT  
		Size: 9.9 MB (9886373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81e748d498b55df670e8577a0fb5193dfd8064fd43c6d2976d7c4543d8a09e6`  
		Last Modified: Tue, 08 Sep 2020 22:30:14 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992ddd9fbe1709be35477ebcfc96360e741bcde325428dd9df90abd9991c44ff`  
		Last Modified: Tue, 08 Sep 2020 22:30:20 GMT  
		Size: 5.3 MB (5339019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42943fb94a665fd49da2a81160ebabd97d68b7bd57cdcf8a10ddeb1947ac2f96`  
		Last Modified: Tue, 08 Sep 2020 22:30:11 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e5a80b0a132994ce5eb9abb9d2a6d63570943944deb7c1d6471667a794eb0c`  
		Last Modified: Tue, 08 Sep 2020 22:30:12 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8919f853d1e44879af394bd54301b0c24f98db2e547a4ddce547fde4d8f2c66b`  
		Last Modified: Tue, 08 Sep 2020 22:30:12 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9edf0bebd7a9ced0b36f319ea331bb03dd8bdc7e55eb9ef2312731d372d54a`  
		Last Modified: Tue, 08 Sep 2020 22:32:41 GMT  
		Size: 201.2 MB (201213599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03d3bbbffd37fb1e1cbe50c4c58ebba12609281aa337c3472823aa43af8e1a8`  
		Last Modified: Tue, 08 Sep 2020 22:30:11 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
