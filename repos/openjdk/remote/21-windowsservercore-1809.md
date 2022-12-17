## `openjdk:21-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:7bbd29541007bc991da47df11a9067a14876b90414ac78c951253388d8a9f26b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `openjdk:21-windowsservercore-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull openjdk@sha256:10763b436afd65bbb13836422d75561bffa06bf6bc647b7cdd64b791d6ca8e85
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (2975652304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:386af96f4cc6206646db5437e40d67cef33f823f0bc365de98e912232bdb39b9`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Tue, 13 Dec 2022 22:48:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Dec 2022 02:52:45 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Dec 2022 02:52:46 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 14 Dec 2022 02:54:02 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 16 Dec 2022 23:22:55 GMT
ENV JAVA_VERSION=21-ea+2
# Fri, 16 Dec 2022 23:22:56 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/2/GPL/openjdk-21-ea+2_windows-x64_bin.zip
# Fri, 16 Dec 2022 23:22:57 GMT
ENV JAVA_SHA256=cde0c6b624e4340dd44950e39e1bd6b5f86fefdf5f3b6367670aafe058a59d65
# Fri, 16 Dec 2022 23:25:12 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 16 Dec 2022 23:25:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9debb9503ac53c2f64685982eca56ac5110ea6baf7278b27af54ab8fbc409`  
		Last Modified: Tue, 13 Dec 2022 23:54:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e607bf43cbd414b2f7d5b6fdfc84e9eb56c2552fe9826cffa690a9d1fd381c`  
		Last Modified: Wed, 14 Dec 2022 08:46:21 GMT  
		Size: 348.4 KB (348396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7bf9dc65d10e90b70525df57c897036594bf31ca9f3291e807694c747e7c0d`  
		Last Modified: Wed, 14 Dec 2022 08:46:21 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3efbe2a37741e8df08f14ef4454b92bc8fbabf777e000dc58fd3642794a700`  
		Last Modified: Wed, 14 Dec 2022 08:46:21 GMT  
		Size: 309.8 KB (309816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406266af6044bd2e9783b77c832cf1a03603fc12b273a276a7987ef1115ad14c`  
		Last Modified: Sat, 17 Dec 2022 02:19:38 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e62ae7222c3776795397d9b9ac2bbea46b60dce8603f74779a2f2566e841260`  
		Last Modified: Sat, 17 Dec 2022 02:19:38 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae63614e791320b6a07440502aba2f1f5dd88c21ad3fa8bcb01b057fe0df7b79`  
		Last Modified: Sat, 17 Dec 2022 02:19:38 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc20f19a6ff2a7e27308e234f02d61dba1fb8b1a0e40ba3dfbd7ee96714a9a1`  
		Last Modified: Sat, 17 Dec 2022 02:20:01 GMT  
		Size: 194.3 MB (194288323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5af20a58d42f5c406832b770f6fef69aa2ab7c3b6a377f147b1f164e072dae7`  
		Last Modified: Sat, 17 Dec 2022 02:19:38 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
