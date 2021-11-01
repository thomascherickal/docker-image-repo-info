## `openjdk:18-ea-21-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:0d5f628a366f1970ccaff603a8ef45066cdbec5bc542aaeda6be7fa6b9eabc29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.288; amd64

### `openjdk:18-ea-21-windowsservercore-ltsc2022` - windows version 10.0.20348.288; amd64

```console
$ docker pull openjdk@sha256:38b89e35ffb038051dbb506694b4f5f0c3b6dc0e1435eea3477e50764c90b964
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2326526811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2b13defe17237b8f7e0a50cf5f5d410c412ffefd6f56962f87f63ffbefd22db`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 07 Oct 2021 11:33:56 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Oct 2021 12:26:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 25 Oct 2021 23:16:39 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Mon, 25 Oct 2021 23:16:40 GMT
ENV JAVA_HOME=C:\openjdk-18
# Mon, 25 Oct 2021 23:17:02 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 01 Nov 2021 18:14:31 GMT
ENV JAVA_VERSION=18-ea+21
# Mon, 01 Nov 2021 18:14:32 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/21/GPL/openjdk-18-ea+21_windows-x64_bin.zip
# Mon, 01 Nov 2021 18:14:33 GMT
ENV JAVA_SHA256=d86fa72089f38517f71cc0bc0b431978c3c5c820971af065f17813249833bd87
# Mon, 01 Nov 2021 18:15:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 01 Nov 2021 18:15:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b03bbc71f9254a4ad2fba472595c859655b9d0cfefa638928416e277e0f0d497`  
		Size: 889.8 MB (889767519 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b201e45e5b11128e36517715f5b6ae98e5782737c1b112a5fae2aa83206f57bf`  
		Last Modified: Wed, 13 Oct 2021 13:23:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a947ce19e17c924828c9323a0de0ab956cabefde1b9245295f097feaff9f13a`  
		Last Modified: Tue, 26 Oct 2021 01:22:57 GMT  
		Size: 628.9 KB (628862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df973053814857f61afa97656cc85bcc253c39d40edf7971e695893f5a006d6f`  
		Last Modified: Tue, 26 Oct 2021 01:22:56 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229e005f3546fff3d9eea6854af9a4671d474eadd333aca8dbebbed48efed762`  
		Last Modified: Tue, 26 Oct 2021 01:22:57 GMT  
		Size: 560.1 KB (560056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f946ab31c6ae6a9a90d576c840049e7b325fb17e320184690fd92d38f0f93a`  
		Last Modified: Mon, 01 Nov 2021 18:24:57 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84474fb107b6ac7f16d3e1565e38aab3b4eb2700984d8d99642a0eb13f21585`  
		Last Modified: Mon, 01 Nov 2021 18:24:57 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d136eed2c64c578d4ffeb7a2b0de9fd969833ad252fe251da10d2f32f90b38`  
		Last Modified: Mon, 01 Nov 2021 18:24:57 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3b501c9d46339773a196f687e9acbf2549e60f397a6b6c873791a154a7ba26`  
		Last Modified: Mon, 01 Nov 2021 18:25:15 GMT  
		Size: 183.9 MB (183862841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6be6b66a589cd87faa618385bd9b2bcef0c72ea43b8d2bea1cff3290197e534`  
		Last Modified: Mon, 01 Nov 2021 18:24:57 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
