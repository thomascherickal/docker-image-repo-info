## `openjdk:14-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:f2bcd5c2f8753f0537d6c2f2a8205f76eb7b7abb9220e90e3a5111b20a73cc97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64

### `openjdk:14-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.3686; amd64

```console
$ docker pull openjdk@sha256:a41f64de1560fe84ea0968fce5e0651cb275cf1a787f8a30c2e79c34eaa730ef
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5941947107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700bacd2d883b93f8200802b3dd0a5d9b3b9dda2e6ce089c30c8733683dc1ac4`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 12:34:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 15:26:34 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 13 May 2020 15:34:51 GMT
ENV JAVA_HOME=C:\openjdk-14
# Wed, 13 May 2020 15:36:06 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 13 May 2020 15:36:08 GMT
ENV JAVA_VERSION=14.0.1
# Wed, 13 May 2020 15:36:09 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk14.0.1/664493ef4a6946b186ff29eb326336a2/7/GPL/openjdk-14.0.1_windows-x64_bin.zip
# Wed, 13 May 2020 15:36:10 GMT
ENV JAVA_SHA256=26255f3f2fe7168ec0dce9d9f3825649c18540ba86279a7506c7f17dd3e537f9
# Wed, 13 May 2020 15:38:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 13 May 2020 15:38:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e3e9730c43354781e87aa51e853bff3b1e8c1ca7004f527139638a8f9d499c49`  
		Last Modified: Wed, 13 May 2020 12:59:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56eaed4a20d0f67d3d00bc23ac486a70424c1d5ebc2b77f4b3bf17c8fcf765d`  
		Last Modified: Wed, 13 May 2020 16:08:25 GMT  
		Size: 5.4 MB (5382606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca4f7e16bf140cf6c0220eec5e496cc4e7624d55d9179ccc4a27c33c201e9d0`  
		Last Modified: Wed, 13 May 2020 16:14:08 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f548990a5fce678899573c85e7e9531f1bc0e3d5c05cd117d33b540378c711e`  
		Last Modified: Wed, 13 May 2020 16:14:14 GMT  
		Size: 5.4 MB (5363205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef34f48a99aa7d1650b2ba126145a3fe91ba310603d2e2aac08e8d608205ee00`  
		Last Modified: Wed, 13 May 2020 16:14:05 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f74ae124dcfd510b1400069bd6470a10c7353d03f4fc40779a00ae3bfd43b0`  
		Last Modified: Wed, 13 May 2020 16:14:05 GMT  
		Size: 1.1 KB (1090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2b26005f965183784f39811d5ff0d37c3f270493e9617800368bed09e516b0`  
		Last Modified: Wed, 13 May 2020 16:14:05 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a215e414068bf78b9661f858140fbb37c60c075d83c0d4f53e03b1bd1cdea65`  
		Last Modified: Wed, 13 May 2020 16:17:54 GMT  
		Size: 199.3 MB (199304789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4af121aca2bead488e14b557fb3157dd5a35344025646d3f7c5a6ec6deb07b9`  
		Last Modified: Wed, 13 May 2020 16:14:05 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
