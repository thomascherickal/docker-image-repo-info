## `openjdk:20-ea-jdk-windowsservercore`

```console
$ docker pull openjdk@sha256:aadd03197d1f3e8960476c2e2be9c0c28ec8ae228ef65dd0872268241e639110
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1129; amd64
	-	windows version 10.0.17763.3532; amd64

### `openjdk:20-ea-jdk-windowsservercore` - windows version 10.0.20348.1129; amd64

```console
$ docker pull openjdk@sha256:cae6644881d20ec3f35e0dc06bc73678d4131a3bd30dcd7bca6cbc240d81469c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668915394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c03d3f739e401d0cb3428859974b960531bf5255304e5b76a1f1fc0c0549e6b7`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:39:02 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:39:03 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 12 Oct 2022 16:39:22 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 07 Nov 2022 21:16:14 GMT
ENV JAVA_VERSION=20-ea+22
# Mon, 07 Nov 2022 21:16:16 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/22/GPL/openjdk-20-ea+22_windows-x64_bin.zip
# Mon, 07 Nov 2022 21:16:17 GMT
ENV JAVA_SHA256=d5cb94516043f93d3117f77a0bfa62cc56c5fa1611ba809e7192f912c3d7f7ad
# Mon, 07 Nov 2022 21:17:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 07 Nov 2022 21:17:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9b54b31e104f64c9eb8a65ac0af5effd645bd00a77ea297b6015d28022a74`  
		Last Modified: Mon, 17 Oct 2022 21:39:11 GMT  
		Size: 1000.0 MB (1000028645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cbc434576dbff410ee0aa4228c6f0fa038ee64fba58d8b81df98ab5bd3e8e5`  
		Last Modified: Wed, 12 Oct 2022 16:51:49 GMT  
		Size: 609.6 KB (609572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d05c1a9fc44de33350221b30e908eaeae6d05eba0fe481490fe562a59dc8fc`  
		Last Modified: Wed, 12 Oct 2022 16:51:49 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71e1244e1a09ac39ec09321d2cf652a948c02d0366d860e30695700811edad3`  
		Last Modified: Wed, 12 Oct 2022 16:51:49 GMT  
		Size: 524.9 KB (524924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28edd116991552a3008e1d9e1e3f35cc3d836248a3ac2b2b71a8284df055602`  
		Last Modified: Mon, 07 Nov 2022 23:18:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55b9e78e9f1348d202fb4b00ea67eaf4238327c1f65fb2e2794c26a1aa6bdc4`  
		Last Modified: Mon, 07 Nov 2022 23:18:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa65b2ae05a569a406f1c939f5c64fcd349000ca8e8be20a6b9a04f279ac95d2`  
		Last Modified: Mon, 07 Nov 2022 23:18:24 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd26711b0604ae894b9e23b13a7cc2e467e63c8c3d5bba16221cc318fb5d0801`  
		Last Modified: Mon, 07 Nov 2022 23:18:46 GMT  
		Size: 193.7 MB (193746076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efc919e85b3ca0c5dbc7122070c748fa97c3a63423b5648b481159d111f4312`  
		Last Modified: Mon, 07 Nov 2022 23:18:24 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk-windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull openjdk@sha256:187146149a82862bf61b3cfed1de1a891e400bb9557e6aa136b11ce836439746
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2967724032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49ef61b4a296fb4af2d959a47fd44ee7dc79ec551c99868b920b0f7a219b28d9`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 16:41:21 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 12 Oct 2022 16:41:22 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 12 Oct 2022 16:42:14 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 07 Nov 2022 21:17:30 GMT
ENV JAVA_VERSION=20-ea+22
# Mon, 07 Nov 2022 21:17:32 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/22/GPL/openjdk-20-ea+22_windows-x64_bin.zip
# Mon, 07 Nov 2022 21:17:33 GMT
ENV JAVA_SHA256=d5cb94516043f93d3117f77a0bfa62cc56c5fa1611ba809e7192f912c3d7f7ad
# Mon, 07 Nov 2022 21:19:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 07 Nov 2022 21:19:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891dd6ec2fa598da717e21a05ad77857caf95e46fc5861ed7e79aab507e9fd11`  
		Last Modified: Wed, 12 Oct 2022 16:52:29 GMT  
		Size: 347.9 KB (347943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e673f50a0247a96d4f10904fad919663c061d29e5445b3531a1eb3a227b99657`  
		Last Modified: Wed, 12 Oct 2022 16:52:28 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f4cce28740d1d55be90dac59ca06df221cfd3100dd82e1eedd5a929a54b2cf`  
		Last Modified: Wed, 12 Oct 2022 16:52:29 GMT  
		Size: 310.8 KB (310762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68e8aa574e95cb48432aea6ea8eb0169edf5eb35879db31e2f71b264dab239d`  
		Last Modified: Mon, 07 Nov 2022 23:19:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10529c251d746e29a983ad3041eb03d8f51e91217903fe65deef834305437cbe`  
		Last Modified: Mon, 07 Nov 2022 23:19:09 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6143c150b071a94b40cf2ecbeed473e7afb1184d4c118f639f4f610ac29146f1`  
		Last Modified: Mon, 07 Nov 2022 23:19:09 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee75f6639c09027efecb7e798c0b488e492219f449abce737a43e91bc0a42cc`  
		Last Modified: Mon, 07 Nov 2022 23:19:30 GMT  
		Size: 193.6 MB (193558468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62b5017d987ef47942ae13c9962e800a4e32979b274391b2179d61371d2e325`  
		Last Modified: Mon, 07 Nov 2022 23:19:09 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
