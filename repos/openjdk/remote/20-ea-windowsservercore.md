## `openjdk:20-ea-windowsservercore`

```console
$ docker pull openjdk@sha256:4703594d80bdfe1b4055eee4fe0f7b42341386a0ca15392076318dbec3f93ebb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1249; amd64
	-	windows version 10.0.17763.3650; amd64

### `openjdk:20-ea-windowsservercore` - windows version 10.0.20348.1249; amd64

```console
$ docker pull openjdk@sha256:1450357f57dd7444b6c87d62d0992200fc9eeec451323220cd821af03b5310be
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2676783890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55e6ad0d151705d05a83c429d49337c5f297889d40bd21f162eaf464d4efeb7d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 17:20:09 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 09 Nov 2022 17:20:10 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 09 Nov 2022 17:20:37 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 18 Nov 2022 01:14:24 GMT
ENV JAVA_VERSION=20-ea+24
# Fri, 18 Nov 2022 01:14:25 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_windows-x64_bin.zip
# Fri, 18 Nov 2022 01:14:26 GMT
ENV JAVA_SHA256=d8045699c2776b155e5266733e02de5568443d48218d346b5c8f648b915038da
# Fri, 18 Nov 2022 01:15:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 18 Nov 2022 01:15:31 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f5ce72a05e01b629001eb0ff2b493ddf6cd8e3c7a836607dc83cfbbec299b3`  
		Last Modified: Wed, 09 Nov 2022 17:35:31 GMT  
		Size: 614.7 KB (614677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766f89a2f9cf276bf435dc9be37e180dfcfc54b750ca8cca41b1e0673eb95abe`  
		Last Modified: Wed, 09 Nov 2022 17:35:30 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3329d7d902a4cde0c4f3848690267bd771e713ccee926c04fc723e62ad0105e8`  
		Last Modified: Wed, 09 Nov 2022 17:35:31 GMT  
		Size: 546.1 KB (546089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c958d24e5cbb7227468de5ba75546bf89af8b680f26609a70f9af1fc740f89`  
		Last Modified: Fri, 18 Nov 2022 01:20:50 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ee11a639d1f03905f593e07c56ec14db5ae44b952b5a7edcd1ceee220e64ef`  
		Last Modified: Fri, 18 Nov 2022 01:20:50 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a36bb205d66f1b13493b2cc58e794b0a2a8ee59ede1c8407e8d4ace773e7234`  
		Last Modified: Fri, 18 Nov 2022 01:20:50 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fac7bad25cea0ebacc0367ef7bdb48b922a65623725fe698d7806b3f325a7dd`  
		Last Modified: Fri, 18 Nov 2022 01:21:11 GMT  
		Size: 193.8 MB (193845954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d66315068f5973532163b90779e9597f6395cfdd5e70bdd37595b1c5f683e25`  
		Last Modified: Fri, 18 Nov 2022 01:20:50 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull openjdk@sha256:841a8f9b0a7ad250f1fd3e36195fa9644c88db9f5b7dc80071c95c51178fbd8c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2972928482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ff311e7c57e6e930757472fcd851fa3361c78448b8864d6f5d5833949a129d3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 17:23:18 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 09 Nov 2022 17:23:19 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 09 Nov 2022 17:24:31 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 18 Nov 2022 01:15:43 GMT
ENV JAVA_VERSION=20-ea+24
# Fri, 18 Nov 2022 01:15:44 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_windows-x64_bin.zip
# Fri, 18 Nov 2022 01:15:45 GMT
ENV JAVA_SHA256=d8045699c2776b155e5266733e02de5568443d48218d346b5c8f648b915038da
# Fri, 18 Nov 2022 01:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 18 Nov 2022 01:17:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c85372c7985a34aa1619da07364507356666af5e2f073a7a04b171c25354b4a`  
		Last Modified: Wed, 09 Nov 2022 17:36:18 GMT  
		Size: 364.8 KB (364807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2c5944c42080bba06b7004a16754ffff768c5ce0b7b3c895891f0f4efe6ef6`  
		Last Modified: Wed, 09 Nov 2022 17:36:17 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e29b6097f3b07473eb77be3c0d8c63285a498161914a045d403afd73a63e73`  
		Last Modified: Wed, 09 Nov 2022 17:36:18 GMT  
		Size: 321.6 KB (321605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e51b3f6c8c1df4c169905529c8bfe505d25615e20b70a57629c6a42a6cae2a0`  
		Last Modified: Fri, 18 Nov 2022 01:21:30 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7ddc5257f0ad56fd7416007698df13f19d941ca1754c5166e93a3b7afb1cb`  
		Last Modified: Fri, 18 Nov 2022 01:21:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e99162f9b909d77edd2ef839cc1bcb31680416d8add514ba8253deef7c004e`  
		Last Modified: Fri, 18 Nov 2022 01:21:30 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9b74589ba715b559f6e445b061983c83d89bf426b684c04f4c1b0ba3fc2366`  
		Last Modified: Fri, 18 Nov 2022 01:21:50 GMT  
		Size: 193.6 MB (193646884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7712f1b6045e3aeb5bcd02c26b10da04f2473dbd95f21248b8ae60307751989a`  
		Last Modified: Fri, 18 Nov 2022 01:21:30 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
