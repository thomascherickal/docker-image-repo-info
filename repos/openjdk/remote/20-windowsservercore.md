## `openjdk:20-windowsservercore`

```console
$ docker pull openjdk@sha256:76324e4657c2b474acb9ad3f27e9fcaa9b88639bd68591822381e8d5d21d3487
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1366; amd64
	-	windows version 10.0.17763.3770; amd64

### `openjdk:20-windowsservercore` - windows version 10.0.20348.1366; amd64

```console
$ docker pull openjdk@sha256:cb86b249742625aa2eb096c773cf80355b2335512357755686a2c159176b475b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690347708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5ed331c9b2e7161ac605c13fcca4ef8c46bf4280200b8e77340482d793ba78`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 09 Dec 2022 09:36:47 GMT
RUN Install update 10.0.20348.1366
# Tue, 13 Dec 2022 22:45:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Dec 2022 02:49:23 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Dec 2022 02:59:12 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 14 Dec 2022 03:00:28 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 16 Dec 2022 23:26:27 GMT
ENV JAVA_VERSION=20-ea+28
# Fri, 16 Dec 2022 23:26:29 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/28/GPL/openjdk-20-ea+28_windows-x64_bin.zip
# Fri, 16 Dec 2022 23:26:29 GMT
ENV JAVA_SHA256=4b3c8da1f2688fa5719498025568253e788381cf47a9d61e93dbad70dbea7292
# Fri, 16 Dec 2022 23:27:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 16 Dec 2022 23:27:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfa20ce142ecceb471dc070d9582fff942cef447b7c8ff22f2223ffe3737c99`  
		Last Modified: Tue, 13 Dec 2022 23:54:14 GMT  
		Size: 1.0 GB (1021665190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb8b9a4ec3ca516cfaa44f64e80b1e3aaecdbde870177411ff046f81f991dd2`  
		Last Modified: Tue, 13 Dec 2022 23:51:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc6d0e6b431095ccd3ac842154ae597a56b82834441570a9c95689f517a56ea`  
		Last Modified: Wed, 14 Dec 2022 08:45:36 GMT  
		Size: 576.9 KB (576869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4228fff1ac4aaf864043ab6ff5341b37ddfbd89a849a638653c590e869dbfa6`  
		Last Modified: Wed, 14 Dec 2022 08:47:59 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7713d48cae58aee42cae5f4e53713018d24ab93530ff940fdadfcfba60393b9`  
		Last Modified: Wed, 14 Dec 2022 08:48:00 GMT  
		Size: 512.9 KB (512898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e404955d12f283cb98c062baf73fe0bfdd95ce0907cc6f591c6d001611af3d4f`  
		Last Modified: Sat, 17 Dec 2022 02:21:00 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4a13dadd6b5c367b80077dbae79898222acf9326cd26914446aaaebf9f562f`  
		Last Modified: Sat, 17 Dec 2022 02:21:00 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb205042edd4173b6c2bebc8dff560edf6c8ac880863c0315538638121471e67`  
		Last Modified: Sat, 17 Dec 2022 02:21:00 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fc056d4c32e87ca8c1a6dda131948dca67e98ae475bf1bb71979db7b63abcd`  
		Last Modified: Sat, 17 Dec 2022 02:21:22 GMT  
		Size: 193.6 MB (193586632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e19efba56f13bcb137503846ae484fb1c867cae39f80b2706b7377f72e6f946`  
		Last Modified: Sat, 17 Dec 2022 02:21:00 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-windowsservercore` - windows version 10.0.17763.3770; amd64

```console
$ docker pull openjdk@sha256:0508c83cbd4a905dc7af5c75b43c53baaa6626ddb9a846b3acdcbaeaf9c3ebba
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2974740964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cbfc44b033d24de364ca2206c02291aa9022aaa55bc7793c8a1f336a805b1d2`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Tue, 13 Dec 2022 22:48:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Dec 2022 02:52:45 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Dec 2022 03:01:57 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 14 Dec 2022 03:03:46 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 16 Dec 2022 23:27:42 GMT
ENV JAVA_VERSION=20-ea+28
# Fri, 16 Dec 2022 23:27:44 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/28/GPL/openjdk-20-ea+28_windows-x64_bin.zip
# Fri, 16 Dec 2022 23:27:45 GMT
ENV JAVA_SHA256=4b3c8da1f2688fa5719498025568253e788381cf47a9d61e93dbad70dbea7292
# Fri, 16 Dec 2022 23:29:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 16 Dec 2022 23:29:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9debb9503ac53c2f64685982eca56ac5110ea6baf7278b27af54ab8fbc409`  
		Last Modified: Tue, 13 Dec 2022 23:54:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e607bf43cbd414b2f7d5b6fdfc84e9eb56c2552fe9826cffa690a9d1fd381c`  
		Last Modified: Wed, 14 Dec 2022 08:46:21 GMT  
		Size: 348.4 KB (348396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e03c14bc9e3d2e4c1490e4b54ba16c12f364ecbabdde8bca9ef0491c8a6398`  
		Last Modified: Wed, 14 Dec 2022 08:48:45 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4c3c241bec90807320674aa89214b5b5dee32c495417743ff949d6c9127020`  
		Last Modified: Wed, 14 Dec 2022 08:48:45 GMT  
		Size: 309.9 KB (309875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27762b070b5c50167e0a9d5a879df3813aec185733d903f295a4f80f80eb5879`  
		Last Modified: Sat, 17 Dec 2022 02:21:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417576f6ad748043e3043646afb674bb70f9be6c8063909d71da35f9bff46246`  
		Last Modified: Sat, 17 Dec 2022 02:21:40 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af335e0085044ea8cde23bd3831a4a457094688e7ae1649324e05840eff1e77c`  
		Last Modified: Sat, 17 Dec 2022 02:21:39 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ca1dc3600e76d7a74da651d482ba06abf62f0b9ce549f537d24cc2048942e5`  
		Last Modified: Sat, 17 Dec 2022 02:22:02 GMT  
		Size: 193.4 MB (193376978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4088480d7782af2bdfb3b89c75a6fea155e9cc951a2f438b8e5d17d15417c7e4`  
		Last Modified: Sat, 17 Dec 2022 02:21:39 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
