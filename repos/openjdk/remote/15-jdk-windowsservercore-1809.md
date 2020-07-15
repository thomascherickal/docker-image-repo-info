## `openjdk:15-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:48d9ad9f9c45c0a8d901eef3e6bd5938b52d99deaea88a002504435b0792aa38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:15-jdk-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:fa1102fa5a201b4b5124e956372807f453156ecc4fc18a94bb22fb8295694824
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2515637849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:278daaff4226ef0500087e60c1df526cadb3de1ee35a5fb9832ac6b24a6786dd`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 01:45:44 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 15 Jul 2020 01:56:24 GMT
ENV JAVA_HOME=C:\openjdk-15
# Wed, 15 Jul 2020 01:56:52 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 15 Jul 2020 01:56:53 GMT
ENV JAVA_VERSION=15-ea+31
# Wed, 15 Jul 2020 01:56:54 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/31/GPL/openjdk-15-ea+31_windows-x64_bin.zip
# Wed, 15 Jul 2020 01:56:55 GMT
ENV JAVA_SHA256=0a97cdf251e6da9f867ba2699332735ce271048bf3213c9355ef078a991d2310
# Wed, 15 Jul 2020 01:58:48 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 15 Jul 2020 01:58:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca5cb7caf11332b67bae426682385af17fa897c718adce9713b111340eb0d71`  
		Last Modified: Wed, 15 Jul 2020 02:42:28 GMT  
		Size: 9.1 MB (9136637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d284b2483b2f168e3ba6ac5972ceaa54db6f335b7cea2a7ba976ec79bceab7`  
		Last Modified: Wed, 15 Jul 2020 02:44:41 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9df741ee75c4cf331249ca7555639e3d621263ed2b077eabfcb7e526e62959`  
		Last Modified: Wed, 15 Jul 2020 02:44:41 GMT  
		Size: 293.0 KB (293037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15303ffca33ffa6ca5a38d92d6e0b7ac6bc954db166e3ea04102ce1f55fe6343`  
		Last Modified: Wed, 15 Jul 2020 02:44:38 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7650757961e8e3cd11a2c98e86d71422ec6e4ac26c26635477a076b31de5279d`  
		Last Modified: Wed, 15 Jul 2020 02:44:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53385f3d7cee9e6b2a0b640edd6d3ce4b98837201328ad18333b80c34ef2001`  
		Last Modified: Wed, 15 Jul 2020 02:44:39 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0531f012b3977e441449f2c16f1994764b57da4e0b18d7ed3dfd5e50da68c2`  
		Last Modified: Wed, 15 Jul 2020 02:45:00 GMT  
		Size: 196.0 MB (196009063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43a50945585eb137d7acbba66247e34a3eb4d0248dfaf7b95f1ed85e97399ad`  
		Last Modified: Wed, 15 Jul 2020 02:44:39 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
