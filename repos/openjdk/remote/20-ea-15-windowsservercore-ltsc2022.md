## `openjdk:20-ea-15-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:cba8cb17a2eca9d173ed3bececed6b0dc80f6493b0b0f7dac1a3e356feab647c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1006; amd64

### `openjdk:20-ea-15-windowsservercore-ltsc2022` - windows version 10.0.20348.1006; amd64

```console
$ docker pull openjdk@sha256:b08d496bbac4bdd761f84b68c2c8bd398674355c712ad72ab85c1cd7b6e6de6d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2540461457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287e2fb1bc1dc3247941057e34312fffa2d6e83fc8bf5778c42b73672d56adb3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:03:52 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Sep 2022 17:03:53 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 14 Sep 2022 17:04:13 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Tue, 20 Sep 2022 23:16:49 GMT
ENV JAVA_VERSION=20-ea+15
# Tue, 20 Sep 2022 23:16:50 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/15/GPL/openjdk-20-ea+15_windows-x64_bin.zip
# Tue, 20 Sep 2022 23:16:51 GMT
ENV JAVA_SHA256=f61766813ba41cd430ef7c20c3e19761919ac9b495e64cda8e8363e9a775f8e9
# Tue, 20 Sep 2022 23:17:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 20 Sep 2022 23:17:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6298a3366175cd1297fbed9781ab93da075956d0549ae06cc0ad3a9f0759b9`  
		Last Modified: Wed, 14 Sep 2022 17:21:32 GMT  
		Size: 593.4 KB (593387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69130dc68926a7dd74a45c56d76c52a89dea16ac92d70aab946e32f9bddfce3d`  
		Last Modified: Wed, 14 Sep 2022 17:21:32 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fc7fa67a5ff75b4568b1c4ae7e98ea07d91433bfd85d115fab3f9d9fd1c762`  
		Last Modified: Wed, 14 Sep 2022 17:21:32 GMT  
		Size: 525.0 KB (524965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cc117f6c6d3bfb9a74fb1b9d89fde53e339140ca111cc7f7844f86e18bb49c`  
		Last Modified: Wed, 21 Sep 2022 00:17:45 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dee3e37a6e753f273e2683c9288c772690561ec320f4cce2afeb2532f3dacab`  
		Last Modified: Wed, 21 Sep 2022 00:17:45 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d89299d4c2eb91948ef5919f84911bd78739bedc504a5452f6d80f95861ccbe`  
		Last Modified: Wed, 21 Sep 2022 00:17:45 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8308eec1a73ac58e66721a05d339b9462c8e14957a3d7933eaf970174c28cdf9`  
		Last Modified: Wed, 21 Sep 2022 00:18:06 GMT  
		Size: 192.4 MB (192385404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70583353d4c0b0dfd072774a4b68919f63f2d060ac8ce819fa5dcfb11f90b6`  
		Last Modified: Wed, 21 Sep 2022 00:17:45 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
