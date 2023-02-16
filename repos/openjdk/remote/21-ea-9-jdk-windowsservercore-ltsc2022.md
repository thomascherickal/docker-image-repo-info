## `openjdk:21-ea-9-jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:79a21b4f6856efafbae8f9e7c9e36910d36a1cfdf2e0fc92e2dfffee44111fad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `openjdk:21-ea-9-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull openjdk@sha256:916c1ccb32c5f8ad0c70280df8730704ad62ff72881056e05b8a4307910b0719
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1875414271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27fb2043f176c73120d5624e3e4af575a06c737dd062c3284e928ed8d6efd15c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:14:39 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:14:40 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 16 Feb 2023 02:15:04 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:15:05 GMT
ENV JAVA_VERSION=21-ea+9
# Thu, 16 Feb 2023 02:15:06 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/9/GPL/openjdk-21-ea+9_windows-x64_bin.zip
# Thu, 16 Feb 2023 02:15:06 GMT
ENV JAVA_SHA256=012fada2a58fa64ab3708ede97876c32050dc6c4dd4c77d29740af88954bda8d
# Thu, 16 Feb 2023 02:16:02 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:16:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8108d16cd884206ec4969828d09af6c32cb29b30d6f5ac0628fbaa03f5acbfc3`  
		Last Modified: Thu, 16 Feb 2023 02:27:56 GMT  
		Size: 770.5 KB (770457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c865bc76fec4cadb1aba9ec04e94e30b1ae91b8396e43f048cac5d9e9751fb`  
		Last Modified: Thu, 16 Feb 2023 02:27:55 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f5b31252c305eec6ed404696a45a13faa4edf1d630169d6b56eb13e25229c`  
		Last Modified: Thu, 16 Feb 2023 02:27:55 GMT  
		Size: 570.8 KB (570829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5308fc3f77ca9348e28d33121478a39592f8693093f9537aa56e6bd002fb75d`  
		Last Modified: Thu, 16 Feb 2023 02:27:52 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fc6fbdd8b38a41cc02ff30637c44fe8663b8ada70dce00ad1818243c079255`  
		Last Modified: Thu, 16 Feb 2023 02:27:52 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d137ced33dfd0fadd0652e297ecbfb586d262527bc12faa25bf2990a01e9c3a2`  
		Last Modified: Thu, 16 Feb 2023 02:27:53 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d01680b0bcb1b4af46c72f6526af6ae70d697a08b11ae95f96353f06848e997`  
		Last Modified: Thu, 16 Feb 2023 02:28:14 GMT  
		Size: 194.7 MB (194718137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12042ede1b9fadbb34038830abb0ee1ca370d1427eadeab4795214adedf3e22`  
		Last Modified: Thu, 16 Feb 2023 02:27:52 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
