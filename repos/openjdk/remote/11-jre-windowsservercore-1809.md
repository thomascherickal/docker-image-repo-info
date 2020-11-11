## `openjdk:11-jre-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:b6f0752dea27d0fe41279fb13c755fb09a98a537c54710d6b353910999fc9b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `openjdk:11-jre-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull openjdk@sha256:b805bdd390981efa2be665a9bbe64805175c70ce0925142b427f05cf7f464349
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2441285252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b481164fcbd97b85144de3a86ef796174dff2cbd257397260c35bd650bd81eec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 18:02:38 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 11 Nov 2020 18:03:18 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Wed, 11 Nov 2020 18:03:19 GMT
ENV JAVA_VERSION=11.0.9
# Wed, 11 Nov 2020 18:10:28 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.9%2B11/OpenJDK11U-jre_x64_windows_11.0.9_11.zip
# Wed, 11 Nov 2020 18:11:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b39c9f3dee64fdf73e852e32e6c2c7d2eb23044e81b2b92f4c0b7a2a60d258`  
		Last Modified: Wed, 11 Nov 2020 18:30:50 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930e6a155975070242394236aad94e80c7b948914e0525aa00fc58acf5f42c81`  
		Last Modified: Wed, 11 Nov 2020 18:30:49 GMT  
		Size: 9.2 MB (9234531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab049a78fab7f64411564d338fd407f0da4c7fc7e58ced051bbd818a00ebf4b`  
		Last Modified: Wed, 11 Nov 2020 18:30:46 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cc730eaa51ad8a25d2ee141ff57732361df968a32d11d5111d255a9326e795`  
		Last Modified: Wed, 11 Nov 2020 18:33:14 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633462a6ad7725b22d7047b23dbd2b6779c2817b0c39c2f906b23f362919ef85`  
		Last Modified: Wed, 11 Nov 2020 18:33:23 GMT  
		Size: 44.0 MB (44016869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
