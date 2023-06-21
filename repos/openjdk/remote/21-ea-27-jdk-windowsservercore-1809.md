## `openjdk:21-ea-27-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:47d289f799af20e452f3c305f94fedc46bf83e11db507092ad3e497936d36e95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `openjdk:21-ea-27-jdk-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull openjdk@sha256:c3bdb529c99912761ee1115d09001c1d4b9dd78e8b14a94b07520565a63b0285
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1849442354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:807cc9ace242e25559e2ed5dd828a55efb671042190ab2e85761d2d756c33640`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 20:26:18 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Jun 2023 20:30:26 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 14 Jun 2023 20:30:53 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 21 Jun 2023 01:58:06 GMT
ENV JAVA_VERSION=21-ea+27
# Wed, 21 Jun 2023 01:58:07 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/27/GPL/openjdk-21-ea+27_windows-x64_bin.zip
# Wed, 21 Jun 2023 01:58:08 GMT
ENV JAVA_SHA256=5bd0a5fae74a966c01bce898d69567bf9bd3e222786dbc2beaf21b2a1df04ef3
# Wed, 21 Jun 2023 01:59:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 21 Jun 2023 01:59:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712a9a082fd391beaa9ca7c8e6c3fda37b0ad8d29cc4663173ed973b961d342`  
		Last Modified: Wed, 14 Jun 2023 18:21:55 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1119c9dd4674cbb889b8cd01bbadf4652797b89d882f89be398f7da1beb24c70`  
		Last Modified: Wed, 14 Jun 2023 20:34:37 GMT  
		Size: 305.5 KB (305458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf3365db6b1a5459442fd3a01aed321cab7afcea801751a10a37b6254119aed`  
		Last Modified: Wed, 14 Jun 2023 20:36:31 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290d337ba15ee034e320e3aab54554a46b97bd5b2abd5b4eabcb81b98112a665`  
		Last Modified: Wed, 14 Jun 2023 20:36:31 GMT  
		Size: 257.3 KB (257292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d80b868fb33d745115e1addca570da01344d717604361747377eb83c2e8386b`  
		Last Modified: Wed, 21 Jun 2023 02:03:48 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37162547a919d4e0e8f0ce6c0cb216cf122e48846dfa8e4b499cca58ca77ab41`  
		Last Modified: Wed, 21 Jun 2023 02:03:48 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d627477e6c1820265602376f3467e575dc5266fcddfca4c6eea78a0d2cabc4`  
		Last Modified: Wed, 21 Jun 2023 02:03:48 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeba5c372c758c57606f8a2c1a8bbefd5d55db591df705cd1e6a1bb5c077c34`  
		Last Modified: Wed, 21 Jun 2023 02:04:09 GMT  
		Size: 198.3 MB (198251266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a5089103a4e5bf482471ed42759c55eddb94731c5d5c8f4dab37ed4d527841`  
		Last Modified: Wed, 21 Jun 2023 02:03:48 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
