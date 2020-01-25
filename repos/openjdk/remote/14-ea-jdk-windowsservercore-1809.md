## `openjdk:14-ea-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:3ba872a39f19a13a0e5cfa62b2e5a35214c8ecd467639f5016c5f01ba090467d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `openjdk:14-ea-jdk-windowsservercore-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull openjdk@sha256:d1d2a6ec368c60b6ca30e1da27e145f79f1de47c77de16191eba3542196574e6
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2416507980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b3b2350b841f2ff06b8cb2dc2c2d44b1cbc998bf2ac5703d161eb08fd9e7927`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Tue, 14 Jan 2020 23:46:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jan 2020 23:47:06 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Tue, 14 Jan 2020 23:58:14 GMT
ENV JAVA_HOME=C:\openjdk-14
# Tue, 14 Jan 2020 23:58:37 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Sat, 25 Jan 2020 04:06:50 GMT
ENV JAVA_VERSION=14-ea+33
# Sat, 25 Jan 2020 04:06:51 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk14/33/GPL/openjdk-14-ea+33_windows-x64_bin.zip
# Sat, 25 Jan 2020 04:06:52 GMT
ENV JAVA_SHA256=4271ae8542f9db36dbe1ab4e716a22a3bcb80c489ee2e87189d8a5c33fb06f15
# Sat, 25 Jan 2020 04:08:48 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 25 Jan 2020 04:08:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9d323e253cb21832421dda4ec57dbd597bd4f934e62c162b9dec8b96e06e818`  
		Last Modified: Wed, 15 Jan 2020 01:45:20 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe8a4080f0d1077681de059bc8597064c929d967b370eac061cacf38283adfe`  
		Last Modified: Wed, 15 Jan 2020 01:45:23 GMT  
		Size: 4.5 MB (4547614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55aa49d97e830f6b3c864cafda1aceff84ee42dab37ddded91a28efb13412be`  
		Last Modified: Wed, 15 Jan 2020 01:55:29 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa48874f549ecadb376734cb21f5139d255704082fc0a269d8667613fa7013c8`  
		Last Modified: Wed, 15 Jan 2020 01:55:29 GMT  
		Size: 289.5 KB (289491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6250c41ae71493dc0aabfcd3a8ead5565946209ca43c0098380d1d221f519b10`  
		Last Modified: Sat, 25 Jan 2020 04:21:19 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2768e76d3f966a94d7d7aef511237d5d4cfdff55d1666c2a8ed36781a195484d`  
		Last Modified: Sat, 25 Jan 2020 04:21:19 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10469570e8c08de1616991fe6f519189bd2cca6a6c6c245acf7128c4ecc8c385`  
		Last Modified: Sat, 25 Jan 2020 04:21:19 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3c00a18e7f8b73e1b85d8d38fd1a3070eaff21d0ca0fd9987942777a8ad6f9`  
		Last Modified: Sat, 25 Jan 2020 04:21:40 GMT  
		Size: 194.3 MB (194252548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0761c6de709e83d88018c0f3ddf03f826efa939c2374773812edaa84bfc1913`  
		Last Modified: Sat, 25 Jan 2020 04:21:20 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
