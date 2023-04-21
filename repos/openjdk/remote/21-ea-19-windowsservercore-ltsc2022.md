## `openjdk:21-ea-19-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:7c38fb453ea43d48f1a3249193b8d00dd91b1bb2db3b01dc3bffb80229fc504a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `openjdk:21-ea-19-windowsservercore-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull openjdk@sha256:cb63d343bf013cdf88337bf697f4d561813d4f61340bfb2787f6feed6055fd13
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1960687186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef0953705fa2135455b54a7aad812a22d86c463a98b42704f8ea7c74fc3c403`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Apr 2023 23:38:34 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Tue, 11 Apr 2023 23:38:35 GMT
ENV JAVA_HOME=C:\openjdk-21
# Tue, 11 Apr 2023 23:39:38 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 21 Apr 2023 19:15:02 GMT
ENV JAVA_VERSION=21-ea+19
# Fri, 21 Apr 2023 19:15:02 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_windows-x64_bin.zip
# Fri, 21 Apr 2023 19:15:03 GMT
ENV JAVA_SHA256=65e4b3cd5a04c50753ee3599a4ea207766ef18e025dab4c38c93403aad9a241e
# Fri, 21 Apr 2023 19:15:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 21 Apr 2023 19:16:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5267a6534dbac53b3d9701ccd066e434901994c544b2dab38b384ba337c288`  
		Last Modified: Wed, 12 Apr 2023 00:49:04 GMT  
		Size: 756.8 KB (756811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec944a3e06641c097fd1420f03d6ca79e689d4e7e7567d6d5220e5722f63c4b`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0fe5145f5a0cc66a5c1d0123eeea45b9ec36dfa42ccfe03d869d89a7bd8416`  
		Last Modified: Wed, 12 Apr 2023 00:49:04 GMT  
		Size: 530.6 KB (530559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9801bcfc7f5cd4870dfffcc5248238419987e4409f0da188731eef11fb3f6ffd`  
		Last Modified: Fri, 21 Apr 2023 19:19:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af15c0a59026202b3aeb5fb29791f6e8ac91e3e9c1b4b1630eea5744087a333`  
		Last Modified: Fri, 21 Apr 2023 19:19:04 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237978c926d01f2beb968c3c6afd0924c12116d1cf2ecaf2cb8da26dd4b705e5`  
		Last Modified: Fri, 21 Apr 2023 19:19:03 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0dcf8f4da270980ae1442fd490d5dd1ae7afd9798fcd0498cbb31cb5a4781a`  
		Last Modified: Fri, 21 Apr 2023 19:19:22 GMT  
		Size: 196.8 MB (196789110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1340bc6daa92850dc0b1b4c5035a82b1380f4c00bcc7ee242ae58d85f72551e`  
		Last Modified: Fri, 21 Apr 2023 19:19:03 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
