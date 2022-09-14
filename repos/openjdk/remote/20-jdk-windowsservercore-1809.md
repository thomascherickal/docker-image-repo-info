## `openjdk:20-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:accb766d8ec5a23e47797e2b5965915da252d609c6401b737f9869b7afb24551
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `openjdk:20-jdk-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull openjdk@sha256:99ec27d11e6059f36000d07b91b9b8413ce404d1da135f20641a328f6dd7b573
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2896374751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ad5d0c0e8c7e214ed956bbc4cfa87a979129096f0e9e31344dcca345a85e59`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 17:06:13 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Sep 2022 17:06:14 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 14 Sep 2022 17:07:14 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 14 Sep 2022 17:07:14 GMT
ENV JAVA_VERSION=20-ea+14
# Wed, 14 Sep 2022 17:07:15 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk20/14/GPL/openjdk-20-ea+14_windows-x64_bin.zip
# Wed, 14 Sep 2022 17:07:16 GMT
ENV JAVA_SHA256=9a074e380bbef6c389a660f1f21bf1cfc449cee8d6c387f4422305b2feb06dc5
# Wed, 14 Sep 2022 17:08:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 14 Sep 2022 17:08:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58648929570c8439cbc01e98ebc75618cbe96e946d332763402b53d89cc5639b`  
		Last Modified: Wed, 14 Sep 2022 17:22:14 GMT  
		Size: 349.5 KB (349457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69dd72d8573f685284949ad83177bf75e72c3d8275d35aa6b4d21f5a480f2b9`  
		Last Modified: Wed, 14 Sep 2022 17:22:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bfc5f723418de82847d7f0e86272a0dc2ec14263a42be94649cbc3d219420b`  
		Last Modified: Wed, 14 Sep 2022 17:22:14 GMT  
		Size: 311.8 KB (311834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c74332a5a503584d141e4d51fe5c24891878edb5aca9cff8fbef7a70bbb9bc1`  
		Last Modified: Wed, 14 Sep 2022 17:22:11 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bb42e8c00a65cd391a35fb34060bb3111bb9338536465c1b1ef51ce2b30ae9`  
		Last Modified: Wed, 14 Sep 2022 17:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5076bfefaa29bfc3cf699f9ef03c810318f793e0b417137518ff8f67dc514d75`  
		Last Modified: Wed, 14 Sep 2022 17:22:11 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eef3cf93097624ee04c6cf1ec59abb673319830a14df2d788886901515bdb7c`  
		Last Modified: Wed, 14 Sep 2022 17:22:31 GMT  
		Size: 192.1 MB (192140231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51c4a517403ec06932069643cc6ae98b4f36d758ab313f44c018830cba7b029`  
		Last Modified: Wed, 14 Sep 2022 17:22:11 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
