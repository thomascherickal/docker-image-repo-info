## `openjdk:19-ea-34-jdk-windowsservercore`

```console
$ docker pull openjdk@sha256:fe864b2e77744f9741608758f2fac7f10534a95b0ae29776ee5dd255a1112013
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `openjdk:19-ea-34-jdk-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull openjdk@sha256:071ab8a578f716bb9c985052536b0916aeb1ab3679fb8943decbaf6f68792e2d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2509841803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3cb1277fe0cbd14d2392e2a1d0dc94e2940ce864e31f7729d05742468a5a8e3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 16:55:00 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 10 Aug 2022 17:01:00 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 10 Aug 2022 17:01:20 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 10 Aug 2022 17:01:21 GMT
ENV JAVA_VERSION=19-ea+34
# Wed, 10 Aug 2022 17:01:22 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_windows-x64_bin.zip
# Wed, 10 Aug 2022 17:01:23 GMT
ENV JAVA_SHA256=5d3ac1a89d92a142588bc8546aa737c37d1971bcff17810b5ff947790c97e623
# Wed, 10 Aug 2022 17:02:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 17:02:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0cc935c154780815cf1fb6065aa1c262b52a7648b984b06133beb4e95833c0`  
		Last Modified: Wed, 10 Aug 2022 17:27:08 GMT  
		Size: 624.7 KB (624700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c321b8aceb5aa354374c98f1ed5eb3ebe9da9235dfb65eaecf437c95f17a9372`  
		Last Modified: Wed, 10 Aug 2022 17:29:18 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06331a3f3c54ed0599c9730f358b1a0548e4df17ed5dc21bacce5929cb4424e5`  
		Last Modified: Wed, 10 Aug 2022 17:29:19 GMT  
		Size: 557.1 KB (557139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6df01a94acd9dc2ffe2ca5fb6a1e7d8da2339fb2dfac3badd2562a04895303`  
		Last Modified: Wed, 10 Aug 2022 17:29:16 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a107949c17d548c8498bd505865892aead1d7a4ee2dde70f9280619b10c12d6`  
		Last Modified: Wed, 10 Aug 2022 17:29:17 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8852ccb6abf7049ca6174c9ae98a324bce09838dcdc08940c2388cef3cb6af8d`  
		Last Modified: Wed, 10 Aug 2022 17:29:16 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee34c08298e6f8f7ea4e4137fff85e2ddf8c24fe9c3d817bee65fd639ff4a1a1`  
		Last Modified: Wed, 10 Aug 2022 17:29:38 GMT  
		Size: 191.8 MB (191762282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c483e898d8717d7eaf30a218bbd8d5a170a89eb170c44265f14bcefea74d75f4`  
		Last Modified: Wed, 10 Aug 2022 17:29:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-34-jdk-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull openjdk@sha256:f3ff49e8e81bd588e87a070b3290289755ebc57d52b2351c78b699fad04facd3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2869901417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df92124d584cac34a8d79cf5890272df1979fdda1c68d9041d20caf1da841513`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 16:57:20 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 10 Aug 2022 17:02:32 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 10 Aug 2022 17:03:26 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 10 Aug 2022 17:03:26 GMT
ENV JAVA_VERSION=19-ea+34
# Wed, 10 Aug 2022 17:03:27 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_windows-x64_bin.zip
# Wed, 10 Aug 2022 17:03:28 GMT
ENV JAVA_SHA256=5d3ac1a89d92a142588bc8546aa737c37d1971bcff17810b5ff947790c97e623
# Wed, 10 Aug 2022 17:04:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 17:04:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9df80b59d75310c5b623001e9a6fefa8c2f0255dfbb8c58e60daa3aba0f9c6`  
		Last Modified: Wed, 10 Aug 2022 17:27:52 GMT  
		Size: 347.3 KB (347323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2c3ccfe82da7c6811a6930391e2fa285e62302c6d82e94343c6c6d13f4dda0`  
		Last Modified: Wed, 10 Aug 2022 17:30:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a1f282d48f602b14cabb59aacdff2e3c30e3c066e3ad20382eb2726f2da1cf`  
		Last Modified: Wed, 10 Aug 2022 17:30:04 GMT  
		Size: 310.2 KB (310237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabc73c37a3f50245266e31a597f90c89e1383a58e14333088f9c30ea70a84c9`  
		Last Modified: Wed, 10 Aug 2022 17:30:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9403325189b7d49b6ac60d15d1d223b10f0eca18612fc58039f09c81b08bb2f5`  
		Last Modified: Wed, 10 Aug 2022 17:30:01 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c01425b0bddb36b098b067ba21dbf220dcc2cb692c7dbd6a25d527022b3eb9d`  
		Last Modified: Wed, 10 Aug 2022 17:30:02 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707c1d9ae00f2ed8401a196654c0351491b62cbe756ef5c74cfabf88d1edc9b1`  
		Last Modified: Wed, 10 Aug 2022 17:30:21 GMT  
		Size: 191.5 MB (191522632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2183152b46a04c9d667bef212bc0a25474637602bbc6709280a3581bd9b05b`  
		Last Modified: Wed, 10 Aug 2022 17:30:01 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
