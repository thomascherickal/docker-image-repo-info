## `openjdk:22-ea-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:00467d9f5d1bf3b67e5ba99555a4fc5596ef76bb1a9405c73388ff7dacd07cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `openjdk:22-ea-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull openjdk@sha256:39be2752bcbc139b75353bd436cc42b5c7bb9bbd79e08c4a0658919c7afdc024
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2231782773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68478d2ebe32c8a552f6bcff303beba7735b1dfb6f9d2575c2ba3e8065f07caf`
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
# Fri, 13 Oct 2023 00:34:33 GMT
ENV JAVA_VERSION=22-ea+19
# Fri, 13 Oct 2023 00:34:34 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/19/GPL/openjdk-22-ea+19_windows-x64_bin.zip
# Fri, 13 Oct 2023 00:34:34 GMT
ENV JAVA_SHA256=44f385f195a458575cc7f87d82c6542188940aaad7840f277ca81e3e407bf4ea
# Fri, 13 Oct 2023 00:36:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 13 Oct 2023 00:36:09 GMT
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
	-	`sha256:f018c28488f0c58881a663272dff6b9d338556a0fa29c63217376ef210108044`  
		Last Modified: Fri, 13 Oct 2023 00:38:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6911c0f95dc6d7e6013d8425d5dc4b78b377e4ce5949e9a95ca036651353d3a`  
		Last Modified: Fri, 13 Oct 2023 00:38:04 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3b3e9c6c459c45fa6ad556d2bd44386a6d0783a1074b627bf5d0fcac4a3c17`  
		Last Modified: Fri, 13 Oct 2023 00:38:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ac7d0e81d321435e0ba83beac1ba52720980f0a6bf6e648d3c099c18bfbaac`  
		Last Modified: Fri, 13 Oct 2023 00:38:23 GMT  
		Size: 199.4 MB (199445773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aea40df1f0f56119c72e9a3c4f63c3369992426d205f4ad8215c3e850c67564`  
		Last Modified: Fri, 13 Oct 2023 00:38:04 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
