## `openjdk:15-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:c1bd59cee642c36ebd2b56491cdd9e18b47278fe1fd5346ffdc61b58e215fe00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `openjdk:15-jdk-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull openjdk@sha256:55b440ed31aac2aa8a4db7426d7b42b7c45f53ec2bccb42598442c75aaf985f3
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2467994620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbc01d4aa1bb1946a7078b2969f3e5b6151c736ba10282b507a14523c25457f8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Apr 2020 21:33:26 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Tue, 14 Apr 2020 21:33:27 GMT
ENV JAVA_HOME=C:\openjdk-15
# Tue, 14 Apr 2020 21:33:53 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 14 Apr 2020 21:33:53 GMT
ENV JAVA_VERSION=15-ea+18
# Tue, 14 Apr 2020 21:33:54 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/18/GPL/openjdk-15-ea+18_windows-x64_bin.zip
# Tue, 14 Apr 2020 21:33:55 GMT
ENV JAVA_SHA256=f5662c45501a71bbc4f90ecc9661a1de3f3813cc8aeacd0d672020d66cc911b0
# Tue, 14 Apr 2020 21:35:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 14 Apr 2020 21:35:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de6b6e18c57fb613f91d77606e5355771830df52cc6b00e32e74a46a7449d5b`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 4.7 MB (4670665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac510bfbe15bdc6d786e0d3d1e28704fc631e945bcce42fb963d86c2f56d0fd8`  
		Last Modified: Tue, 14 Apr 2020 22:15:54 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0176aea199d3313340042e173fe6b28bc5a463a889d351a42f25db76d678ebf6`  
		Last Modified: Tue, 14 Apr 2020 22:15:55 GMT  
		Size: 295.7 KB (295672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff67b7d98d4ea5c9eee2e51f153d090ea93288fca43a2381924d832b843cc4e`  
		Last Modified: Tue, 14 Apr 2020 22:15:52 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833f36e3abc270a37ce23c8626103e291419bc33e014caf8f684ea3cadb7adcc`  
		Last Modified: Tue, 14 Apr 2020 22:15:52 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c29edee265d43f4ad2688bddd64aa30a7101dc99bafc301b56e014b67d6df77`  
		Last Modified: Tue, 14 Apr 2020 22:15:53 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff075a3dfa91bda47bf91e352397e14f928160f1dbe2247ae6c95871142615b`  
		Last Modified: Tue, 14 Apr 2020 22:16:12 GMT  
		Size: 192.3 MB (192314406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16d5f57138cf611c1ffec62089952a738a4ba7e8a3fd6dda4e59bd9b0eb2a24`  
		Last Modified: Tue, 14 Apr 2020 22:15:52 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
