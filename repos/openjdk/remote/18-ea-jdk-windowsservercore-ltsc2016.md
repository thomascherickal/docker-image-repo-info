## `openjdk:18-ea-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:5a702ce0f76b8bc4c7add1f6d6b915032ad23773329aea470784787fc29eee3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `openjdk:18-ea-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull openjdk@sha256:5e5504eb78653397c3a31af7b8e19191c6149f2090b26d5c7df9f1d79095dcfa
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6455238682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e365d877ab8c63f988e14c7337dc58303ed9b1e72fe6ba85383a6631512113`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 00:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 00:35:51 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 15 Sep 2021 00:35:52 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 15 Sep 2021 00:36:45 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 17 Sep 2021 19:31:49 GMT
ENV JAVA_VERSION=18-ea+15
# Fri, 17 Sep 2021 19:31:50 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/15/GPL/openjdk-18-ea+15_windows-x64_bin.zip
# Fri, 17 Sep 2021 19:31:51 GMT
ENV JAVA_SHA256=bd0121a79be31881084e84d41a16f8be15692ab5dd4cd4736d9bd7d67700dc75
# Fri, 17 Sep 2021 19:33:21 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 17 Sep 2021 19:33:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8721f004192f15fe71b8626ef3f3e34cbf2cfe1d15a63b6b544ab946162ef707`  
		Last Modified: Wed, 15 Sep 2021 01:10:18 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b794d0a07a41196dae8678e4ecbb9a5766d6db31f9729bfe3f1d83963af3e0`  
		Last Modified: Wed, 15 Sep 2021 01:10:18 GMT  
		Size: 339.2 KB (339172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d3bfbbd6119f5d4c8cdfa80560f7d1dfa6730c4d5af995fee76f3decd44528`  
		Last Modified: Wed, 15 Sep 2021 01:10:17 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8da815f1cb98dfe565a92045b7ed382138e2c7bbbba2982c14bcecce8161396`  
		Last Modified: Wed, 15 Sep 2021 01:10:17 GMT  
		Size: 335.9 KB (335946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d0441b64bfd162e0c790e69d86f0f948208d5cc86f2d3c6231c4d1198f5885`  
		Last Modified: Fri, 17 Sep 2021 19:41:55 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26a1fa87f3a557d52f2956bc69ea2e560e5029d43a9fe7c152cbaef0de8eebe`  
		Last Modified: Fri, 17 Sep 2021 19:41:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782165ac1acea3e41b26f75000618203211f45a3721b8779e27ffc919891a513`  
		Last Modified: Fri, 17 Sep 2021 19:41:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2de87d84b52034c7d605db8f9c2f852a148379950e89e4b0314a66319e516f6`  
		Last Modified: Fri, 17 Sep 2021 19:42:13 GMT  
		Size: 183.2 MB (183227044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01f3702ad5a86965aa3621c22b9b02e4685106d80c8344fdf7443dac76f4be6`  
		Last Modified: Fri, 17 Sep 2021 19:41:56 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
