## `openjdk:16-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:f94c403b50722ac4801c40e6f1069df4dcdfb5947f1b4d61cca7a4daf8625d0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `openjdk:16-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull openjdk@sha256:6ba3abc94a2e0bf0ebd7d3d97ae2be083f053b807b0345d309a39022894e2f78
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5941620513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4e12c83e316d60c6e3567fd2cf54b32409c9c9185d24655ee0c5dc3df29348`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Jun 2020 22:36:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 09 Jun 2020 22:38:24 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Thu, 18 Jun 2020 21:16:57 GMT
ENV JAVA_HOME=C:\openjdk-16
# Thu, 18 Jun 2020 21:18:09 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Mon, 22 Jun 2020 19:16:43 GMT
ENV JAVA_VERSION=16-ea+2
# Mon, 22 Jun 2020 19:16:44 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/2/GPL/openjdk-16-ea+2_windows-x64_bin.zip
# Mon, 22 Jun 2020 19:16:45 GMT
ENV JAVA_SHA256=7694c25b10335e5e4fe1dc1f9e51d11f551dfa9deb65e7a5f487ce105547fc3a
# Mon, 22 Jun 2020 19:19:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 22 Jun 2020 19:19:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c938241e0507e1ada5f864325483d86fd08533a5a31e7cb6ec1357db9891b245`  
		Last Modified: Tue, 09 Jun 2020 23:18:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20399ac1a4e75ca1edbca4b2438a810ea66dbe6bdd128414ab987881b5ed641`  
		Last Modified: Tue, 09 Jun 2020 23:18:34 GMT  
		Size: 5.4 MB (5393368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0dd9264ba0994a55b3b3e6ec6de6aa7a3cc79e9631fdc64a7d415862c6e663`  
		Last Modified: Thu, 18 Jun 2020 21:27:38 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045e933fb92f211c0340e61df32c43c09514287233ce23cb21180ca616fbd25e`  
		Last Modified: Thu, 18 Jun 2020 21:27:39 GMT  
		Size: 5.4 MB (5381916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63612f3a3c5d23105c81156aae22a7f005ccf3059e47fad872c41067b89037f0`  
		Last Modified: Mon, 22 Jun 2020 19:31:27 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ce4a4a7fad7c5d87e918b103afc2e521a122c3748bd7d64e17fb9005b40920`  
		Last Modified: Mon, 22 Jun 2020 19:31:26 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6db315082ae0df5c05b05373344d6e68ea76a525cd634b1b7e76c5bb7558e1`  
		Last Modified: Mon, 22 Jun 2020 19:31:27 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e9a61e6bdaaed7a477d41d2196fadae419a097f5dc06157ccd27f4b6bfe02`  
		Last Modified: Mon, 22 Jun 2020 19:31:50 GMT  
		Size: 196.8 MB (196840672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4ba5b2fb299c686ce288f8143b7f3ca083da895f7d34b7ebc0024023be5fa3`  
		Last Modified: Mon, 22 Jun 2020 19:31:27 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
