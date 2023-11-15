## `openjdk:22-ea-23-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:2143e44136dae82fbef5465202c52520a49e8a2ffa1e03334e48b89d6fd805f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `openjdk:22-ea-23-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull openjdk@sha256:673dd9163795316fd093198589e5e3dbe786b6e26cdf4140edd501c3987567dc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2232630796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cd2104b4c0d6ffd6a833f1844bbf46088b0b02c3d4331963456809c970734c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:51:39 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 11 Oct 2023 03:51:40 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 11 Oct 2023 03:52:38 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 15 Nov 2023 03:43:16 GMT
ENV JAVA_VERSION=22-ea+23
# Wed, 15 Nov 2023 03:43:17 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/23/GPL/openjdk-22-ea+23_windows-x64_bin.zip
# Wed, 15 Nov 2023 03:43:18 GMT
ENV JAVA_SHA256=25e3fa403b5e501bf5e66189205dd806161aeef87a3a35b861fa3f46ab286852
# Wed, 15 Nov 2023 03:45:40 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 15 Nov 2023 03:45:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f783cb3f1b4d13355b852dedee9d6d4d1970fb4493dc1642d1b2a2f2e81e868b`  
		Last Modified: Wed, 11 Oct 2023 03:56:26 GMT  
		Size: 460.2 KB (460193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130ee22501b1f092f84a96a93216a4e26e770e6728f3298841b909959eed064c`  
		Last Modified: Wed, 11 Oct 2023 03:56:26 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d71937d13c516a2428fe61543786cb08bd8e9b4ddf3d0bd80582d9e54be7950`  
		Last Modified: Wed, 11 Oct 2023 03:56:26 GMT  
		Size: 278.1 KB (278058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dff676e63952dd6c130cce10aea4b87c5abeea19c96f71e25434851f750b79`  
		Last Modified: Wed, 15 Nov 2023 03:48:11 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9587cad6e3f74ad84f3912d63bfbaf20edbaf146db0694cbaae86a9caa163f5e`  
		Last Modified: Wed, 15 Nov 2023 03:48:11 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c842442c5f5bdff3733c542c6d7942524aab164ecb7306b08463894a8dfa4aa`  
		Last Modified: Wed, 15 Nov 2023 03:48:11 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a06ee5dc202a7abce6e9b4b03e62e98e0422d356ca9e12f0f70811b6b8e634`  
		Last Modified: Wed, 15 Nov 2023 03:48:37 GMT  
		Size: 200.3 MB (200293750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6065b1b3901f8668ff0443a8b65aecaca3a2f523ca1eba9cf0587833692f7f56`  
		Last Modified: Wed, 15 Nov 2023 03:48:11 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
