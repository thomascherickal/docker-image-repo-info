## `openjdk:22-ea-2-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:0efe12deacf31cbab89c1efe6a28b7f42d9db2d8c4a75585dd72e92817d0533b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `openjdk:22-ea-2-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull openjdk@sha256:b32c8a0349070552bc564eb5b1f0c5460a01eb06c3247060eee432766ffb4817
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1850207291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3a0422c5a77ea66a8f405896ee5317b8a3e7a0ea03afb957a4272faf73e23c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:39:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 20:26:18 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Jun 2023 20:26:18 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 14 Jun 2023 20:26:44 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 21 Jun 2023 01:55:10 GMT
ENV JAVA_VERSION=22-ea+2
# Wed, 21 Jun 2023 01:55:11 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/2/GPL/openjdk-22-ea+2_windows-x64_bin.zip
# Wed, 21 Jun 2023 01:55:12 GMT
ENV JAVA_SHA256=5c387014bc480e9bc3e204504d0fcd933912694e6a4a44c044696e4f2a9b7ca1
# Wed, 21 Jun 2023 01:56:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 21 Jun 2023 01:56:11 GMT
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
	-	`sha256:ba9ed58112430e156afd8c7eed20069147a2b5ecdb1b8da57264db5ea41dd214`  
		Last Modified: Wed, 14 Jun 2023 20:34:37 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e32d8326ab7a8f29c3209f83dfd8c39f6746f5de5efc42d984740194104030`  
		Last Modified: Wed, 14 Jun 2023 20:34:37 GMT  
		Size: 257.0 KB (257037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965e8c631beb60dc4a2573c7906abfebfbbb06781bde7f8e493b3006d7a412ca`  
		Last Modified: Wed, 21 Jun 2023 02:01:42 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0af91f5aff4e61b492e6f218ad7c502a79f5635b237bb58b02b555d7fbe753`  
		Last Modified: Wed, 21 Jun 2023 02:01:42 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0d2cb4731cb2801e1ba958a1ede0e9ffe410e07e43693d8a7075c9b48aff99`  
		Last Modified: Wed, 21 Jun 2023 02:01:43 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6809970a6d8591ae7a4d0ba4d5c71c7bf697726578fa2793b8b654034c586ac`  
		Last Modified: Wed, 21 Jun 2023 02:02:04 GMT  
		Size: 199.0 MB (199016511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca1b74485c4d82db797e33391572be3cda60a985220e9e0029075386c25e6c2`  
		Last Modified: Wed, 21 Jun 2023 02:01:42 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
