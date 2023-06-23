## `openjdk:21-ea-jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:73aed4874345debc8402130c2dd8e226a90fdd9a20aa8dbe2fbb4233e0c830b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `openjdk:21-ea-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull openjdk@sha256:b0e77461e9eb0fe50af377b590b015d0795991f2532c2fcd85923d19b6c01436
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1587435509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15e9943fc62cfb56836d7e20785d590349c62f1debbea5cc44aec130c6877ad`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 17:38:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 20:24:17 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Jun 2023 20:28:58 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 14 Jun 2023 20:29:22 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 23 Jun 2023 00:37:31 GMT
ENV JAVA_VERSION=21-ea+28
# Fri, 23 Jun 2023 00:37:32 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/28/GPL/openjdk-21-ea+28_windows-x64_bin.zip
# Fri, 23 Jun 2023 00:37:33 GMT
ENV JAVA_SHA256=cf31047fdf44c7303408c4868c810af10ec573e926925041e621f0d5acca4583
# Fri, 23 Jun 2023 00:38:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 23 Jun 2023 00:38:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972ddd233121a2afd2cf1a3eaec49d595cfe6b3ebe19ef3dd492d99784c370f`  
		Last Modified: Wed, 14 Jun 2023 18:17:55 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ecf7cfdecc4064a3b0d43346d08171233c7f384d58889a6b8710f45b5c57a9`  
		Last Modified: Wed, 14 Jun 2023 20:33:59 GMT  
		Size: 318.3 KB (318286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebbdd7b332be16a3a5df77e0a2c4d72833fdacc6a2cab0bd336093650ded15a`  
		Last Modified: Wed, 14 Jun 2023 20:35:53 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a57ea6f3fe157301ffb86456c425db57163025371e05b4c02e81c1d7e25d56`  
		Last Modified: Wed, 14 Jun 2023 20:35:53 GMT  
		Size: 263.4 KB (263355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6eb45f1d750943200be960ef462371fdb6c0d83097108da8f6688a81df098e0`  
		Last Modified: Fri, 23 Jun 2023 00:43:22 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c7bdf7e878de4d1c47cc22b95f3ed1379e344d41405ba271fefe076a16a240`  
		Last Modified: Fri, 23 Jun 2023 00:43:22 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92201423bd46eeef1354f60b8a450e86663af5d1d5a6b1490b0e68f439c10a`  
		Last Modified: Fri, 23 Jun 2023 00:43:22 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce6f5ab338bf5231c2371b28d1b26190ac138ae3a75084b6cc38d08e5527e3b`  
		Last Modified: Fri, 23 Jun 2023 00:43:42 GMT  
		Size: 198.2 MB (198246908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267ce274510fbfae753634a5dccac05f1337080c901b38a4676a698cb424981`  
		Last Modified: Fri, 23 Jun 2023 00:43:22 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
