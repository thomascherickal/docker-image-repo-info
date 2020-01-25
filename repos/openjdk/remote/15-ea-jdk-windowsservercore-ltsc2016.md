## `openjdk:15-ea-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:e5995bedc4832b31dd9b18adde2f753327c68c1ac604f8c9656698fff5972af3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `openjdk:15-ea-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.3443; amd64

```console
$ docker pull openjdk@sha256:57162ac62a7a203ce3e211de3ecd748b3ae8e72f6adfc3ee4c4510950143bd4f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5934742936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8dfb261cf954411015a5bc332381eb9c4db076e907d0c00635e28a61dd6fcb8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jan 2020 23:50:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Jan 2020 23:51:57 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Tue, 14 Jan 2020 23:51:59 GMT
ENV JAVA_HOME=C:\openjdk-15
# Tue, 14 Jan 2020 23:53:12 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Sat, 25 Jan 2020 04:02:13 GMT
ENV JAVA_VERSION=15-ea+7
# Sat, 25 Jan 2020 04:02:15 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/7/GPL/openjdk-15-ea+7_windows-x64_bin.zip
# Sat, 25 Jan 2020 04:02:16 GMT
ENV JAVA_SHA256=43e95b54566cdc58ec11ec778a37e9563a4bb8771fcd3af4f39380ff99d7c6d0
# Sat, 25 Jan 2020 04:04:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 25 Jan 2020 04:04:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f1c8c4c99f36cfcf87884a9382011e93fb05fa4002d8f4eca62a43e744db8e95`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59f69707d10b5be4e5c56881ea890fd476325bea3b16b5a7e7c56a1d8b3f056`  
		Last Modified: Wed, 15 Jan 2020 01:46:54 GMT  
		Size: 5.4 MB (5386027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13be2a284f8df11c1998bfd13983fd3023d2ab26119d0573b5d1da6b0bc517b5`  
		Last Modified: Wed, 15 Jan 2020 01:46:47 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9dc4dd3193169ca67387a679b62b0f258cdfed78e25069276beeefb16957e68`  
		Last Modified: Wed, 15 Jan 2020 01:46:49 GMT  
		Size: 5.4 MB (5368228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1a351c43b56346608e9da47ef222c053155625416977502776187fbf42f58a`  
		Last Modified: Sat, 25 Jan 2020 04:18:38 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d286a4a2737d2638af4b55ea9cded900fcbcfd9d5e09eb7bea61f57fdfa8be9`  
		Last Modified: Sat, 25 Jan 2020 04:18:37 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23ad838763679115e5af0c6aee24acdfcc5a5af02a3a5ed9a5db806469f3c95`  
		Last Modified: Sat, 25 Jan 2020 04:18:37 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e8434733d80c6854d1033e2337d7021b59b9555491308b47730b39224342e0`  
		Last Modified: Sat, 25 Jan 2020 04:18:59 GMT  
		Size: 199.4 MB (199382273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0bc0c24b46db7a583fc52ef23dd426a5558136943915af8274be538cfcdcba`  
		Last Modified: Sat, 25 Jan 2020 04:18:37 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
