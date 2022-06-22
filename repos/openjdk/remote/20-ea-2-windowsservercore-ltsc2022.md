## `openjdk:20-ea-2-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:a43c57c07109e422ac8396ad4925141dbec88268dabc3508976356d3ecb1fa26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.768; amd64

### `openjdk:20-ea-2-windowsservercore-ltsc2022` - windows version 10.0.20348.768; amd64

```console
$ docker pull openjdk@sha256:8fc38cd3880bcb448cb8f2b2b24ef533797727b80d0c02b0c72de8495625002f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2472447604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adbb28b1e51f4b7e7cb19a56ae454cc670c788b7e146461dbe154ea3536ae71`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 09 Jun 2022 04:32:50 GMT
RUN Install update 10.0.20348.768
# Wed, 15 Jun 2022 12:13:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 19:30:14 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Jun 2022 01:14:39 GMT
ENV JAVA_HOME=C:\openjdk-20
# Thu, 16 Jun 2022 01:15:08 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 22 Jun 2022 00:43:45 GMT
ENV JAVA_VERSION=20-ea+2
# Wed, 22 Jun 2022 00:43:46 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/2/GPL/openjdk-20-ea+2_windows-x64_bin.zip
# Wed, 22 Jun 2022 00:43:47 GMT
ENV JAVA_SHA256=8dc5a274cd002d32ae4c8f6561afb4b620763ac5c05a3fdf77ea1b5ad58fbe3a
# Wed, 22 Jun 2022 00:44:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 22 Jun 2022 00:44:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c71967ff41928927e4c407171e4ffbac3c9ab4221eb64f5ca5a34ff4c230567`  
		Size: 841.6 MB (841600427 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dec0338feaf01f35eb916b7fd9ecc08b719354163254885d5215e513c1a3eb2e`  
		Last Modified: Wed, 15 Jun 2022 12:49:26 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b6e059d50cccbff94037bf242f1b94acf1cc939d701dff58c07f4fcfdc9767`  
		Last Modified: Wed, 15 Jun 2022 20:02:04 GMT  
		Size: 632.3 KB (632288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e4ff554b66055922423d154f7282c8144066ebe31d1393200cf475fb56555f`  
		Last Modified: Thu, 16 Jun 2022 01:26:02 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a207dedd7fa079f899254dd9a6ea4b20cbb4e77f9880ed19716901e210c1e42f`  
		Last Modified: Thu, 16 Jun 2022 01:26:02 GMT  
		Size: 564.2 KB (564202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b410becae28da98cf3dfbe89961fdce7d06d4e812eb2754adbf8ac5090962fe1`  
		Last Modified: Wed, 22 Jun 2022 02:21:01 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f56547dc781f34bf6b9287fffa681df757f3b6e937f2811c39b7a99f2e316ed`  
		Last Modified: Wed, 22 Jun 2022 02:21:01 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7f521e26920b4cbbee7d688f2af6d24a6b12287fd13729549d71844d181902`  
		Last Modified: Wed, 22 Jun 2022 02:21:01 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59fc63ab696ebb1e274427cc28de05c3092d1c87f39ef3613b9f7a61c2d2c42`  
		Last Modified: Wed, 22 Jun 2022 02:24:31 GMT  
		Size: 192.8 MB (192778565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f31263e29428da3a257cdae2ba85cf98403b88c97552bc06ed1aab791d2b0a`  
		Last Modified: Wed, 22 Jun 2022 02:21:01 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
