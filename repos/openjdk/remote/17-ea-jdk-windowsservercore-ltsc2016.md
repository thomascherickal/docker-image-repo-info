## `openjdk:17-ea-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:bc010386274f78fe4bcd1cff11b4cf3ed1534518eb4d0e03adb3e4dda887efff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `openjdk:17-ea-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull openjdk@sha256:67f3ae50cb61afdebfd48d444eb8820040487cb41c231446e22b589d52f82f5a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5980160127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa43ec1cdc33d3119606c079597f728bf991c49f1865341cf40678aaee0c93a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 18:53:57 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Mon, 28 Dec 2020 21:47:41 GMT
ENV JAVA_HOME=C:\openjdk-17
# Mon, 28 Dec 2020 21:48:54 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Mon, 28 Dec 2020 21:48:55 GMT
ENV JAVA_VERSION=17-ea+3
# Mon, 28 Dec 2020 21:48:56 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk17/3/GPL/openjdk-17-ea+3_windows-x64_bin.zip
# Mon, 28 Dec 2020 21:48:57 GMT
ENV JAVA_SHA256=6208dba1b22a0c2cbe91bf4073bf19b551c402667b71bbaa4f91ab0445b89e5a
# Mon, 28 Dec 2020 21:51:17 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 28 Dec 2020 21:51:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535454b21129910f68c2c2c0ef15ca3640eb529cf7325adda5148aa9a68bc914`  
		Last Modified: Wed, 09 Dec 2020 19:33:19 GMT  
		Size: 10.0 MB (10046782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0955884b499a3e3f215d69d2e5c6f62b2b69c6ee539558c63f06cb56201012d`  
		Last Modified: Mon, 28 Dec 2020 22:01:58 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bb5abb319de65fb1e86e37ab29031c5f2de7db41cbd93d54993c873730847c`  
		Last Modified: Mon, 28 Dec 2020 22:02:00 GMT  
		Size: 10.0 MB (10015465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae08af36035e2447dd9db0a79244d8a9308cd41201b6be2a0d71cd36e6a3872`  
		Last Modified: Mon, 28 Dec 2020 22:01:54 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc1281475ef0ddda16bfbfd0a7b0cd41bfa46c9461a271d853c8d0b7cbae994`  
		Last Modified: Mon, 28 Dec 2020 22:01:53 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d27ccd3246f17281c3d488e6486abe42a5b036301bc2e81c8cab1c28c8fd49`  
		Last Modified: Mon, 28 Dec 2020 22:01:54 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f117bc2e87f2dc6f48efc7316ee460f916cff64ff732ed21579e0ed324316010`  
		Last Modified: Mon, 28 Dec 2020 22:02:32 GMT  
		Size: 191.2 MB (191247049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ba64a2828b36e70a1dcf9ee1b6f9e8e80dd96845e7f36c69cafeffb6a966db`  
		Last Modified: Mon, 28 Dec 2020 22:01:54 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
