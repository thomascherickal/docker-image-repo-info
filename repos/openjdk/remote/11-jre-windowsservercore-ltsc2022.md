## `openjdk:11-jre-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:c983c865bdd12d9853578b7c628386e08d6f74161e066f923f1e92254429de0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.288; amd64

### `openjdk:11-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.288; amd64

```console
$ docker pull openjdk@sha256:f75d44fd39608415c77c8764a21ad7e302520379467409c22ae5cbf2d118cc3b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2182650419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b2a8f08343da276d2ca4a64b1af88a4d603c28f2eb941a200dd37f12ac479bc`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 07 Oct 2021 11:33:56 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Oct 2021 12:26:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 25 Oct 2021 23:16:39 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Mon, 25 Oct 2021 23:21:07 GMT
ENV JAVA_HOME=C:\openjdk-11
# Mon, 25 Oct 2021 23:21:28 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 25 Oct 2021 23:21:29 GMT
ENV JAVA_VERSION=11.0.13
# Mon, 25 Oct 2021 23:23:02 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jre_x64_windows_11.0.13_8.zip
# Mon, 25 Oct 2021 23:23:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b03bbc71f9254a4ad2fba472595c859655b9d0cfefa638928416e277e0f0d497`  
		Size: 889.8 MB (889767519 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b201e45e5b11128e36517715f5b6ae98e5782737c1b112a5fae2aa83206f57bf`  
		Last Modified: Wed, 13 Oct 2021 13:23:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a947ce19e17c924828c9323a0de0ab956cabefde1b9245295f097feaff9f13a`  
		Last Modified: Tue, 26 Oct 2021 01:22:57 GMT  
		Size: 628.9 KB (628862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4735c45400143ec5b3b1edaef3b3187ec8cb9f154d8a622c4cbb50a1a293212`  
		Last Modified: Tue, 26 Oct 2021 01:27:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94111437fdc5cece862338d88683b0c19be5e137bcdd1b93787be3aa39f75dae`  
		Last Modified: Tue, 26 Oct 2021 01:27:52 GMT  
		Size: 560.3 KB (560318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42fb8f9e36f5e5fe95c6a8423364ee89d217225a761690fc63c8d58e251e93e0`  
		Last Modified: Tue, 26 Oct 2021 01:27:52 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a815a5aeb2fedfa0c0a120bafa3024cc21f34dc208ceb4d71ce445a614fa38`  
		Last Modified: Tue, 26 Oct 2021 01:28:42 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59d70bf8df94ed0248a1a73b584c376ab73e695abc6c97bf2324168981e2fb9`  
		Last Modified: Tue, 26 Oct 2021 01:28:51 GMT  
		Size: 40.0 MB (39988970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
