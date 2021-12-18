## `openjdk:18-ea-28-jdk-windowsservercore`

```console
$ docker pull openjdk@sha256:23fc0ebf8b644a8cc721e8acd8a0680475cde18dc0230cafc131c399d1235d99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `openjdk:18-ea-28-jdk-windowsservercore` - windows version 10.0.20348.405; amd64

```console
$ docker pull openjdk@sha256:95a9aa65e10b23fffc2bf9a9bd5588ee81d8ac151370f9b82cec6638c8445018
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2376448384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1daafcf1559b23f559ea42c407293b723f89782ad2abeb91f9234481095a4feb`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 08 Dec 2021 01:54:07 GMT
RUN Install update ltsc2022-amd64
# Sat, 18 Dec 2021 00:09:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 06:52:31 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Sat, 18 Dec 2021 07:03:46 GMT
ENV JAVA_HOME=C:\openjdk-18
# Sat, 18 Dec 2021 07:04:17 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 18 Dec 2021 07:04:18 GMT
ENV JAVA_VERSION=18-ea+28
# Sat, 18 Dec 2021 07:04:19 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_windows-x64_bin.zip
# Sat, 18 Dec 2021 07:04:20 GMT
ENV JAVA_SHA256=f074b562a232f67574a3aa0e5402f82540c1c7e1bfc9050ef6e6e4f145b81bb6
# Sat, 18 Dec 2021 07:05:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 07:05:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d1d74adc6a92e44b3cd592ec9459f1fff926eaf6fc20bb7526360bec71aefc0`  
		Size: 939.1 MB (939072515 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5bc74beb7593c703ac99379d225f3a9a445549cc06a3fe18f44e356a45f225f3`  
		Last Modified: Sat, 18 Dec 2021 01:18:31 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8faf6738034b8742c8193d3db825f75f650b85ef03ad87a2f9e6d91f195c38d2`  
		Last Modified: Sat, 18 Dec 2021 10:51:31 GMT  
		Size: 635.1 KB (635126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33616cf8971399858dc392d3e603c9a6c4eff8c6054af2d8492d250b300756b9`  
		Last Modified: Sat, 18 Dec 2021 10:57:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1a684c0e994a86f11bcc0f30830fad11b052093f81257505ce6a25ecac099`  
		Last Modified: Sat, 18 Dec 2021 10:57:14 GMT  
		Size: 544.5 KB (544523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc1d1cabf5776bfe7a35374ba56e87f1951293da182fe9c95025bdb5aaed972`  
		Last Modified: Sat, 18 Dec 2021 10:57:11 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346da0ad075a843d23b864f6543b27f915079d9fe2a146005a47590857a6e898`  
		Last Modified: Sat, 18 Dec 2021 10:57:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc33b7ad8556ab7d0e20601ad3ae7a7873384fc744d907b7c952f1384c4ddb2`  
		Last Modified: Sat, 18 Dec 2021 10:57:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3338f2c06decd924b51c267d3e4e707ad0b4fdae8ae293f6855b3e7d52ca679b`  
		Last Modified: Sat, 18 Dec 2021 11:00:28 GMT  
		Size: 184.5 MB (184488619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0b87f6fced947c78b3a3a7066ed566cda6c212bc6854e15c7e20488fe3e904`  
		Last Modified: Sat, 18 Dec 2021 10:57:11 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-28-jdk-windowsservercore` - windows version 10.0.17763.2366; amd64

```console
$ docker pull openjdk@sha256:4481b652c36491ee6f8e9e781b89106592c468209199267c47cad903dab18f0e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2893619460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9719f4712a3383276b56cf80d1b714751d4ca0638ffd36560b7013a1847bee18`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Fri, 17 Dec 2021 23:26:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 06:56:01 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Sat, 18 Dec 2021 07:05:28 GMT
ENV JAVA_HOME=C:\openjdk-18
# Sat, 18 Dec 2021 07:06:51 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 18 Dec 2021 07:06:52 GMT
ENV JAVA_VERSION=18-ea+28
# Sat, 18 Dec 2021 07:06:53 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_windows-x64_bin.zip
# Sat, 18 Dec 2021 07:06:54 GMT
ENV JAVA_SHA256=f074b562a232f67574a3aa0e5402f82540c1c7e1bfc9050ef6e6e4f145b81bb6
# Sat, 18 Dec 2021 07:08:23 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 07:08:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31b2acce136e44984ba36d64717a6a67fbf1a98ed7ffcf0a14df848c1502a345`  
		Last Modified: Fri, 17 Dec 2021 23:47:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ef2f84414aadaa12189f793787857287076489d28b83d8f44727621fdc6793`  
		Last Modified: Sat, 18 Dec 2021 10:55:13 GMT  
		Size: 374.2 KB (374167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb03ce95f5cb3cf434995496d5e9199741f2e3ff4ebb26880dca6013069e4bc`  
		Last Modified: Sat, 18 Dec 2021 11:00:50 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5741bbbde36f0dd0d1d665d728713acd13cf9f256fdabc6940ed4a6488fc67d7`  
		Last Modified: Sat, 18 Dec 2021 11:00:50 GMT  
		Size: 337.5 KB (337467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a4f994004625d44aef8017d25ce0746fef08cdfebf004993f6767e9f72ac19`  
		Last Modified: Sat, 18 Dec 2021 11:00:47 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d52f4b3e85496670460cac0e8cfb77b02621315f794e1b813e00ef48476c49`  
		Last Modified: Sat, 18 Dec 2021 11:00:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b30f685e97f9c3e1fb1fa7411da4acae9a828cfc25633f1f58c31afdb858a9e`  
		Last Modified: Sat, 18 Dec 2021 11:00:47 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05141d87b39f888a1b84d62358421c0caa7e02601e0b2fa3cdb7907af9828085`  
		Last Modified: Sat, 18 Dec 2021 11:04:12 GMT  
		Size: 184.3 MB (184294848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8518ab8f5d39280c45b7429d6fb801f4f76f8d5b6517eb99f41f1e22d4ba7daf`  
		Last Modified: Sat, 18 Dec 2021 11:00:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-28-jdk-windowsservercore` - windows version 10.0.14393.4825; amd64

```console
$ docker pull openjdk@sha256:6bd35bbd868341ed46bc9a8c16792a8299664cc372c3d3e3795c1e6d4ec1f8c2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6459646808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71d0ef48f2075793024a87dd4422d238901697f24f1d610dfb77cbcfb9f9b86`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 06:59:56 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Sat, 18 Dec 2021 07:08:40 GMT
ENV JAVA_HOME=C:\openjdk-18
# Sat, 18 Dec 2021 07:09:56 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 18 Dec 2021 07:09:57 GMT
ENV JAVA_VERSION=18-ea+28
# Sat, 18 Dec 2021 07:09:58 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_windows-x64_bin.zip
# Sat, 18 Dec 2021 07:09:58 GMT
ENV JAVA_SHA256=f074b562a232f67574a3aa0e5402f82540c1c7e1bfc9050ef6e6e4f145b81bb6
# Sat, 18 Dec 2021 07:11:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 07:11:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f88306d11f630889687486bb566861161592f87bc40ac9850fce316e5b7780`  
		Last Modified: Sat, 18 Dec 2021 10:55:53 GMT  
		Size: 335.8 KB (335827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b6cd0c0ddb275bff04e82262e96ff042aa7e6340d0b8a3adce915bef0331d2`  
		Last Modified: Sat, 18 Dec 2021 11:04:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0311e7beac3446508723ce8cebedd1494521d0143b567d476b6e8ecb9d690d9b`  
		Last Modified: Sat, 18 Dec 2021 11:04:35 GMT  
		Size: 330.2 KB (330217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b19fc54fe132361579ff3136a563918d2d954fe561e7f793aeb0afca9c0eaf6`  
		Last Modified: Sat, 18 Dec 2021 11:04:32 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7908e23022203bc261404ed1872e2b8525d14a46f8aaee23371fd4c8f1382a49`  
		Last Modified: Sat, 18 Dec 2021 11:04:32 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc47b2235d160d853386dce0bd0c3c02fca96efaa4177533ee5067b56a28640`  
		Last Modified: Sat, 18 Dec 2021 11:04:32 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99bc61c2081cd9a397fbe700fae44d9e24bc59a2b1f906c282006b6d283ea17`  
		Last Modified: Sat, 18 Dec 2021 11:07:44 GMT  
		Size: 184.3 MB (184257496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b673dc6039492ce96bfb9f052cb1aa15b442ebca8c19c2494bb29bfc76bc83`  
		Last Modified: Sat, 18 Dec 2021 11:04:32 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
