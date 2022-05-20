## `openjdk:19-ea-jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:3e24d22b306326ccea1ff549e3cea6e21cdfd0ec6ae8a5b674bcc0b1ecc0e58f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `openjdk:19-ea-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull openjdk@sha256:dcfc992928d7afaef075af0a87b6b1abd4f2819fc437f51d1d8c95f0456a18ea
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2429868606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4f74600516bf2194cba1abf8759129e46665e045063e154d0a5816049a51416`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 15:28:55 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 11 May 2022 15:28:56 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 11 May 2022 15:29:16 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 20 May 2022 21:15:34 GMT
ENV JAVA_VERSION=19-ea+23
# Fri, 20 May 2022 21:15:35 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/23/GPL/openjdk-19-ea+23_windows-x64_bin.zip
# Fri, 20 May 2022 21:15:36 GMT
ENV JAVA_SHA256=d86c8cd64a8563ff063cc3b7e2fadcbee2e96066cc1a443397ae01274bc8300d
# Fri, 20 May 2022 21:16:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 20 May 2022 21:16:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7320671bb1ef07c493563d61e332d907b7a248c0d182698a877d84e65327b614`  
		Last Modified: Wed, 11 May 2022 15:56:04 GMT  
		Size: 607.9 KB (607907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c59d468f4140dfeb9ca7cccc1a19de4b9dee810da486843372bc823daddb570`  
		Last Modified: Wed, 11 May 2022 15:56:03 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613b2526877fb3edad53c027ade0fb2feb1ec41cfe4a7bfc4d5d1db891b391e5`  
		Last Modified: Wed, 11 May 2022 15:56:04 GMT  
		Size: 539.4 KB (539446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52f83bd5e9e770a63380ba7ca2e3994e763e99861ce60cebb205faecb6c65e0`  
		Last Modified: Fri, 20 May 2022 21:24:06 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9611001de99f76ee02a929d56bc9aa4981baf3e50ef50c6816b8298a47859248`  
		Last Modified: Fri, 20 May 2022 21:24:06 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336a3a58ccd52916cc054826dc492d0d8fc0b0be35f0ac75b1932ac107abb6a6`  
		Last Modified: Fri, 20 May 2022 21:24:06 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3107e82fc21aa3f5cb8a6f769b956a1d440c66e435d7305e7dc5031f893338d0`  
		Last Modified: Fri, 20 May 2022 21:27:31 GMT  
		Size: 191.2 MB (191177525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04748cd0779599a44d02112d10e28ebbe5a79050797d49a74d22e752c239fd87`  
		Last Modified: Fri, 20 May 2022 21:24:06 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
