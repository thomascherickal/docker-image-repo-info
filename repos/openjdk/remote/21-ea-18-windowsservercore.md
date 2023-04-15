## `openjdk:21-ea-18-windowsservercore`

```console
$ docker pull openjdk@sha256:b6f2c0a2f8650150fd0dabb8ba1810f652d7a49e85affae5e076747f05050684
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1668; amd64
	-	windows version 10.0.17763.4252; amd64

### `openjdk:21-ea-18-windowsservercore` - windows version 10.0.20348.1668; amd64

```console
$ docker pull openjdk@sha256:e53485a5ae00af19eadd6d7c10ac03b74861beacc31390097ccc210aa62bac30
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1960529476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4df85365e3fac91e4c1610244609c981bb189c6347b38742acd8b733868e4775`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Apr 2023 23:38:34 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Tue, 11 Apr 2023 23:38:35 GMT
ENV JAVA_HOME=C:\openjdk-21
# Tue, 11 Apr 2023 23:39:38 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 15 Apr 2023 00:22:43 GMT
ENV JAVA_VERSION=21-ea+18
# Sat, 15 Apr 2023 00:22:44 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_windows-x64_bin.zip
# Sat, 15 Apr 2023 00:22:45 GMT
ENV JAVA_SHA256=b7e51c6a8bc99197d95429e462cf7025dacb4eb4709d0f6f231cc2cec76e17b3
# Sat, 15 Apr 2023 00:23:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 15 Apr 2023 00:23:34 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5267a6534dbac53b3d9701ccd066e434901994c544b2dab38b384ba337c288`  
		Last Modified: Wed, 12 Apr 2023 00:49:04 GMT  
		Size: 756.8 KB (756811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec944a3e06641c097fd1420f03d6ca79e689d4e7e7567d6d5220e5722f63c4b`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0fe5145f5a0cc66a5c1d0123eeea45b9ec36dfa42ccfe03d869d89a7bd8416`  
		Last Modified: Wed, 12 Apr 2023 00:49:04 GMT  
		Size: 530.6 KB (530559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084b68c56c0eab67f9c3e0e8ed08524f95948ce27d03296d72f4a98ec3683e50`  
		Last Modified: Sat, 15 Apr 2023 00:26:57 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96781573ad55f31b7f19685bca3e0e2b77ad497d969cc2cd0d5b63080924ca6c`  
		Last Modified: Sat, 15 Apr 2023 00:26:57 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95816fbc465a74d5d3f36007cddee868f89e5787d7d255f79cd0ce0b47b3c97a`  
		Last Modified: Sat, 15 Apr 2023 00:26:57 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb4af452744bf87b162450fb741206a656c7e3e0df25d3b876b06fd790f64af`  
		Last Modified: Sat, 15 Apr 2023 00:27:16 GMT  
		Size: 196.6 MB (196631509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc30e298f798a9c022ac4747661e146844565ececfb1eec479c653598a4a50c6`  
		Last Modified: Sat, 15 Apr 2023 00:26:57 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-18-windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull openjdk@sha256:578e7c84204a425f96cb954f96a9c695312742670b86b84e48786ae718cdb0f7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2268521728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cea0a0bf150bd95215b1fa4578a688ee5d165abffec5c933ce947308f1e439f3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Apr 2023 23:42:24 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Tue, 11 Apr 2023 23:42:25 GMT
ENV JAVA_HOME=C:\openjdk-21
# Tue, 11 Apr 2023 23:43:30 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 15 Apr 2023 00:23:45 GMT
ENV JAVA_VERSION=21-ea+18
# Sat, 15 Apr 2023 00:23:45 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_windows-x64_bin.zip
# Sat, 15 Apr 2023 00:23:46 GMT
ENV JAVA_SHA256=b7e51c6a8bc99197d95429e462cf7025dacb4eb4709d0f6f231cc2cec76e17b3
# Sat, 15 Apr 2023 00:25:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 15 Apr 2023 00:25:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2a17e347e3144ab020e098f925bc273e89f499e03114bea80260a0bc601f9c`  
		Last Modified: Wed, 12 Apr 2023 00:50:56 GMT  
		Size: 487.7 KB (487655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c03d658bc6a61ee9591db424ef2db8137173e1ff03e628327eda8134490cb46`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4c3c308ea664c1238fc40d20ade9c94a79f29169edf764c414e542fc4495ab`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 311.4 KB (311449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1237cc3a1d5ae777bc904e9aaac57193efcb36f923ea2d101bdb6816307e230c`  
		Last Modified: Sat, 15 Apr 2023 00:27:34 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a47734d513312309be1e294e669babf04f4a25e3a237ad1c37f7a986d8ab288`  
		Last Modified: Sat, 15 Apr 2023 00:27:34 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fcf16add4c650168a22c905ed730860f18dbc596a17fb7ce240f7d81577d165`  
		Last Modified: Sat, 15 Apr 2023 00:27:34 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d35f9b434d41f4737ae5516829bc29f86f4eedbab72206269a6f1e357da5d5`  
		Last Modified: Sat, 15 Apr 2023 00:27:54 GMT  
		Size: 196.4 MB (196422851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba9bb8545d8f6469e9fa4608a669abeb2d004b85c801d7f7753eb50fc124a7`  
		Last Modified: Sat, 15 Apr 2023 00:27:34 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
