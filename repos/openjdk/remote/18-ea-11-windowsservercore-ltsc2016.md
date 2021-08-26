## `openjdk:18-ea-11-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:0e5194fdb916269f4acce089c6367e9334bc3b97808a95bedeb56746f6da0207
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `openjdk:18-ea-11-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull openjdk@sha256:0e46d27867becc5d43aeeb0fa76d124e144ec2482da2864b73d6c5a98c735e3d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6454604555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65262e3c9d82eab9cd32a3a101f34e445e2b3c915f111f5bd21ea3603d9e83b2`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 17:03:58 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 25 Aug 2021 17:03:59 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 25 Aug 2021 17:04:55 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 25 Aug 2021 17:04:56 GMT
ENV JAVA_VERSION=18-ea+11
# Wed, 25 Aug 2021 17:04:57 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/11/GPL/openjdk-18-ea+11_windows-x64_bin.zip
# Wed, 25 Aug 2021 17:04:58 GMT
ENV JAVA_SHA256=ec68ebcdbca228f5360163b7f0c7338764cae1f5ca1b3240726cf23e67e0ab7f
# Wed, 25 Aug 2021 17:06:24 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 25 Aug 2021 17:06:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd31633f2d1c2da743d0885711cbfa9104d68fe4decd491c7f0ca6964213546`  
		Last Modified: Thu, 26 Aug 2021 00:39:17 GMT  
		Size: 342.3 KB (342299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e17ff82e1afec12110d1011e396cbb2620559aaedd9bbca3f2aab973f00d86`  
		Last Modified: Thu, 26 Aug 2021 00:39:17 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7551d92777c2d65fde1b1593722f052df49cde1ef847e71a5fe136229697d257`  
		Last Modified: Thu, 26 Aug 2021 00:39:18 GMT  
		Size: 335.4 KB (335430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16f702024e6bcf0c785386ec7ff9bd1110465f488db19475800fed04069ad23`  
		Last Modified: Thu, 26 Aug 2021 00:39:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a692e59801ff8952e86d206cb1356d7760e09dd2a22b0e30c13b67a0684e7d`  
		Last Modified: Thu, 26 Aug 2021 00:39:14 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68382771336d0e4d2e93a5aa816f389a9766c28d2afb83b049072858979e6daa`  
		Last Modified: Thu, 26 Aug 2021 00:39:14 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571c683bbf2b5f493a5fa4a6eab5c1978118794f25c9e0db6df2ec685221f7af`  
		Last Modified: Thu, 26 Aug 2021 00:39:34 GMT  
		Size: 183.0 MB (182952805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dded9e97143ef66cbece7cc4bbfe379dea158781fd85885b20042537af0e79`  
		Last Modified: Thu, 26 Aug 2021 00:39:14 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
