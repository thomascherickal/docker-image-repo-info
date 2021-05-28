## `openjdk:17-ea-24-windowsservercore`

```console
$ docker pull openjdk@sha256:e580a6fed9b5503ba56a5ff8e721ca7acdb8b3a16471d2cdbee86520e00c836b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `openjdk:17-ea-24-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull openjdk@sha256:20f486affb402b1af70f9bd14404c365f1e8603e8a16bd69076dcad6d3c788b0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2661424806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:246c47e8b29433cab4cc02656a1f9adf1119e3706981b0a116331ab3400b4bb6`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 16:35:37 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 12 May 2021 16:35:38 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 12 May 2021 16:36:03 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 27 May 2021 23:14:33 GMT
ENV JAVA_VERSION=17-ea+24
# Thu, 27 May 2021 23:14:34 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/24/GPL/openjdk-17-ea+24_windows-x64_bin.zip
# Thu, 27 May 2021 23:14:35 GMT
ENV JAVA_SHA256=b19feaa3767bf8389684b5e41f5d012882625c3fff6a2a039bcc71471275ae71
# Thu, 27 May 2021 23:16:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 27 May 2021 23:16:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed0a49f151d983ea76d28f662a09813d5519c713f8356278fc4506a48465166`  
		Last Modified: Wed, 12 May 2021 17:15:05 GMT  
		Size: 5.1 MB (5099027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adaa80926e62caa127e4c259e0e5b4ac2701bc636194e0cb724847945fb39a7a`  
		Last Modified: Wed, 12 May 2021 17:15:03 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6159e0915c6c5d2d1daba1e45f935dbfd9b5f03a4a0b1b53947ede04b91f41e3`  
		Last Modified: Wed, 12 May 2021 17:15:04 GMT  
		Size: 307.3 KB (307274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d0b2e488d6a28760fe94c50f189a4bc5b0fc389dc1f60e9a9683ae6ed65d42`  
		Last Modified: Thu, 27 May 2021 23:25:58 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a06328a7bb6969a7fcc04d36f586c418da3686cb60da516c8d67d48d8a1574`  
		Last Modified: Thu, 27 May 2021 23:25:58 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df921243b6828d9b12a65064253b8f5e49ec909c3cae08a1888ee8334cb0d59`  
		Last Modified: Thu, 27 May 2021 23:25:58 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23a9cda3e6fb180bddaa28ee7e7508d14ca995dd8c65a8d14d7edb4dc96391`  
		Last Modified: Thu, 27 May 2021 23:26:17 GMT  
		Size: 181.5 MB (181521314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ca2626604c365e6b3539950c99167c5630a80ac4314bbd9f9a0df41d977bf9`  
		Last Modified: Thu, 27 May 2021 23:25:58 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-24-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull openjdk@sha256:752083ee6d30f1dbbf4e90c40541386509d27fafcd8428fca7f144906ba69d99
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5993963628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a6815f6d1ae6cf8cefbf7963c27bf855b0a9a9fda3a5be77d36870eb53630d1`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 16:38:48 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 12 May 2021 16:38:49 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 12 May 2021 16:40:27 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 27 May 2021 23:16:45 GMT
ENV JAVA_VERSION=17-ea+24
# Thu, 27 May 2021 23:16:47 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/24/GPL/openjdk-17-ea+24_windows-x64_bin.zip
# Thu, 27 May 2021 23:16:48 GMT
ENV JAVA_SHA256=b19feaa3767bf8389684b5e41f5d012882625c3fff6a2a039bcc71471275ae71
# Thu, 27 May 2021 23:18:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 27 May 2021 23:18:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e207924c83ffdb1664a8c8f2d8914f8ac2d146d0a5eec997b2c359ff33d928`  
		Last Modified: Wed, 12 May 2021 17:15:54 GMT  
		Size: 5.7 MB (5704156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a2dd60a2ba0434a7771edebc5672a533b07697e2e838edf0a81b78018a9b7e`  
		Last Modified: Wed, 12 May 2021 17:15:51 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a8ab2abad565743f1605667a5a908cdf299295c156e49d7fd0af878b56920f`  
		Last Modified: Wed, 12 May 2021 17:15:53 GMT  
		Size: 5.6 MB (5647985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4473b58392602c7d27795ddce32e817cc4c5e6ab4acb05b55409c1abc8c40108`  
		Last Modified: Thu, 27 May 2021 23:26:39 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afb530b290742d6c3a9f70e383e7dbfc80cc2b63eb3ff34d0bb2a3e4bbb0456`  
		Last Modified: Thu, 27 May 2021 23:26:39 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430b32fd48261cbec201d0752ad0e78b0493d12865c824f0e9cebc8a50070806`  
		Last Modified: Thu, 27 May 2021 23:26:39 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d055c5b3fe29ae6aa56216cdb0d1014e55558ec3525b51e766db110181b9071`  
		Last Modified: Thu, 27 May 2021 23:27:01 GMT  
		Size: 186.8 MB (186825989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5110af3c80fbfe4b6d25e8a8a8989ef9b400724d46a3cd19759131eac9d4b1`  
		Last Modified: Thu, 27 May 2021 23:26:39 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
