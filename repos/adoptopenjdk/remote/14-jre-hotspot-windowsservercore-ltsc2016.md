## `adoptopenjdk:14-jre-hotspot-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:fd1351574786e41b3b05bc006e772dffc40d2e46afa03070e56ba4084d69a07d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `adoptopenjdk:14-jre-hotspot-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull adoptopenjdk@sha256:a4a182a614d40e228968b1c13e68e635a558d4c04441002cf93a5f03de4324e2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5844587907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:925eaf34a7c99f918ed31a1b63459ae3d9270baef354f825daaffcf56cfc8667`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 19:28:08 GMT
ENV JAVA_VERSION=jdk-14.0.2+12
# Wed, 14 Oct 2020 19:36:42 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jre_x64_windows_hotspot_14.0.2_12.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jre_x64_windows_hotspot_14.0.2_12.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (bf468c78387b8095914a2d46af6961d5c22697929b66961e346a41fc8bf909d4) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'bf468c78387b8095914a2d46af6961d5c22697929b66961e346a41fc8bf909d4') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3685603ccf52c648bccad78e97a5b2519fb7c160445169e7e0ce6d9a47950d79`  
		Last Modified: Wed, 14 Oct 2020 20:29:12 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac1369c338ca7960968664dccd781d91a8960fd825cb38fd2ca8c92a59a1771`  
		Last Modified: Wed, 14 Oct 2020 20:31:23 GMT  
		Size: 103.2 MB (103233954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
