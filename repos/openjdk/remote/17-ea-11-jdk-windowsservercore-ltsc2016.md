## `openjdk:17-ea-11-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:f07f6d2792d1de56df0d9418564b9aac43270ab1c2ce07119a42462fd8fad1a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `openjdk:17-ea-11-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull openjdk@sha256:bcea601e945b4efb4b138ac19831498f3155977389b70171841c01b5a89cdb1b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6001997478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21341fb449541731650cc74470273e048e4ff349af2cfb653c37afcd70674da9`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Feb 2021 13:17:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Feb 2021 16:42:35 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 10 Feb 2021 16:42:36 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 10 Feb 2021 16:43:46 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 26 Feb 2021 21:16:53 GMT
ENV JAVA_VERSION=17-ea+11
# Fri, 26 Feb 2021 21:16:54 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/11/GPL/openjdk-17-ea+11_windows-x64_bin.zip
# Fri, 26 Feb 2021 21:16:55 GMT
ENV JAVA_SHA256=3c86c308ca0449d0fd6d6504b6038d97fe9ef16b63cb97540081c492849d6b40
# Fri, 26 Feb 2021 21:18:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 26 Feb 2021 21:18:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c03f1c41641d4a4cf6906dee9a590ee67135d926dddab80cfef993cae745a38a`  
		Last Modified: Wed, 10 Feb 2021 13:41:36 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852b6d2d8c5b49e04837d97a06dfd545d620e2355d40bc0014a563f58a5c11c2`  
		Last Modified: Wed, 10 Feb 2021 17:16:55 GMT  
		Size: 10.2 MB (10165560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9c4a33cf4184ec2758f116995a1883c4e175af9c2087923a3e8073b0380068`  
		Last Modified: Wed, 10 Feb 2021 17:16:51 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27a6f1b8e5829537ed39d3d76ff8d153d99087fc769b430652f6c539854ea31`  
		Last Modified: Wed, 10 Feb 2021 17:16:52 GMT  
		Size: 5.6 MB (5613663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05254e245c14af200532a0a966cdb0f0d578b84b317ef302ed4091ca07147298`  
		Last Modified: Fri, 26 Feb 2021 21:26:38 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa7e2b5a6805219c86eaf3a4789552dd129c12591877b024c0d34800a1106a5`  
		Last Modified: Fri, 26 Feb 2021 21:26:38 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17ceb6d0589ff95c29337c7bceea530ec61a6593dd2168f0c085c426d3347df`  
		Last Modified: Fri, 26 Feb 2021 21:26:39 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcc877a255f5d9174dbec6f768d79d987bbc4303161713bad613970557e9eea`  
		Last Modified: Fri, 26 Feb 2021 21:30:19 GMT  
		Size: 191.2 MB (191196805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0b8f4a2e1f528fe0a528e5936167b44e2d6816f1fd433fe2e40f1723f5f198`  
		Last Modified: Fri, 26 Feb 2021 21:26:38 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
