## `openjdk:19-ea-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:ff775361d7716a264df728f5295770e6eaf8df799ed4614029e141ad28d214b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `openjdk:19-ea-jdk-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull openjdk@sha256:2301231afbedfdcb09b85e5e9f688694517e7cc3cea5636233e29c4a4cc1f5b3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2906673174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a0036c6af4cc272f5b13ab8267c0dcf90f6275683bb1a6d2b89f84cf1cb80c6`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 16:58:06 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Apr 2022 16:58:07 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 13 Apr 2022 16:59:01 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 25 Apr 2022 18:23:14 GMT
ENV JAVA_VERSION=19-ea+19
# Mon, 25 Apr 2022 18:23:16 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_windows-x64_bin.zip
# Mon, 25 Apr 2022 18:23:17 GMT
ENV JAVA_SHA256=ce58fcc89396bc21321e1b8359fe9310124a65b9e94664befe215e35f4ad9789
# Mon, 25 Apr 2022 18:26:00 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 25 Apr 2022 18:26:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25b7048e3be90e8d3856a943edfe91e214649883ffeabdf6fcebcea7b3053e2`  
		Last Modified: Tue, 19 Apr 2022 00:53:10 GMT  
		Size: 366.7 KB (366674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f218e98479db3f32c0db578928d63948fc1a4d83a3525921b9f9a7f4c999de53`  
		Last Modified: Tue, 19 Apr 2022 00:53:09 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4898bdb62896a1acbb34025e03c775d3d5f0f7299ae3f01875842d74e0e7984b`  
		Last Modified: Tue, 19 Apr 2022 00:53:10 GMT  
		Size: 322.4 KB (322423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4c821de8c5ead6594322e587331cb2fbf4fc60caed2ca9e61d26b8027aa09b`  
		Last Modified: Mon, 25 Apr 2022 20:21:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70eb77e016384cd3a52baef0a876fff58450e4aed1500da4aecc68b63dbd53a3`  
		Last Modified: Mon, 25 Apr 2022 20:21:57 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b94c54a5aaa57f9c3fd22e9854ecca2dccf901d578e658fcb063d883f899fb`  
		Last Modified: Mon, 25 Apr 2022 20:21:57 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7ce0792e22dfa20430335e2063d245b306e99dbc193fdbef9c0b0abcc54916`  
		Last Modified: Mon, 25 Apr 2022 20:25:26 GMT  
		Size: 190.1 MB (190055224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bf80642549dfef1d2cc63a5ab7347d25fb256a7ba527690dd3d43655da7a37`  
		Last Modified: Mon, 25 Apr 2022 20:21:57 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
