## `openjdk:18-ea-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:84a723ef710bda45ec1c2fbe8c0b98c6c36a748279dab1487c4c81df83d62fe8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `openjdk:18-ea-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull openjdk@sha256:b5d72a07d0abafca8a0e3121657354de31ec6d7099ebe8db74c8b81654638c0e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6455399364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:686fa0d8ac6005bdee8081ed534f397fecb852c0ce598c71d9e4735c589f82e1`
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
# Sat, 25 Sep 2021 00:17:10 GMT
ENV JAVA_VERSION=18-ea+16
# Sat, 25 Sep 2021 00:17:11 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/16/GPL/openjdk-18-ea+16_windows-x64_bin.zip
# Sat, 25 Sep 2021 00:17:12 GMT
ENV JAVA_SHA256=d59e49abb435e202744d954994789e87302a9bed870f889241a5774d4ef6db31
# Sat, 25 Sep 2021 00:18:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 25 Sep 2021 00:18:56 GMT
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
	-	`sha256:62da6b07d6b37caff1befab67598d487ec5e2dbbbeea127741fdbcc5796f97cc`  
		Last Modified: Sat, 25 Sep 2021 00:28:22 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3ea5b791d84af39e48a509b17d7be69c7b65c925066b11091e704bd55e6893`  
		Last Modified: Sat, 25 Sep 2021 00:28:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4400aacec1fc782a21efe2c7ac606dd9d688a7d996d7b5bf5138836e563add17`  
		Last Modified: Sat, 25 Sep 2021 00:28:22 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5649e4141e669e5bdb98962f5358c0c1200d407585c36160bf10e49b3e2311a0`  
		Last Modified: Sat, 25 Sep 2021 00:31:31 GMT  
		Size: 183.4 MB (183387742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c92519e95b5424f0be72e20ac527ab7686865b1b28b6982cd5b9d07d5504d54`  
		Last Modified: Sat, 25 Sep 2021 00:28:18 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
