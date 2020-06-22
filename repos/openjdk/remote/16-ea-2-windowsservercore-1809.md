## `openjdk:16-ea-2-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:5e15bd4053d28341c1df584fd6b2f3ca7f75034482dc19d70492208e2b39e0fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `openjdk:16-ea-2-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull openjdk@sha256:c4485ba0f726e0e20eaf88e7312ff0090e4fdb4b294542e2c7532695a6328f25
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2490726126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74375d68f9045026ac88fa46fffe4de1b1367d1cdf0c603cccc1afaf9bfeac8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Tue, 09 Jun 2020 22:33:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 09 Jun 2020 22:34:11 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Thu, 18 Jun 2020 21:14:30 GMT
ENV JAVA_HOME=C:\openjdk-16
# Thu, 18 Jun 2020 21:14:54 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Mon, 22 Jun 2020 19:14:46 GMT
ENV JAVA_VERSION=16-ea+2
# Mon, 22 Jun 2020 19:14:48 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/2/GPL/openjdk-16-ea+2_windows-x64_bin.zip
# Mon, 22 Jun 2020 19:14:48 GMT
ENV JAVA_SHA256=7694c25b10335e5e4fe1dc1f9e51d11f551dfa9deb65e7a5f487ce105547fc3a
# Mon, 22 Jun 2020 19:16:30 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Mon, 22 Jun 2020 19:16:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f841c6a0c622cd36b5b2688011a224ac3e8e96273758f4a2804f2f3f099f267d`  
		Last Modified: Tue, 09 Jun 2020 23:17:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d8ec06304524cdb2b900879af7ed2db71d5e36e5f2306b46859250255390d`  
		Last Modified: Tue, 09 Jun 2020 23:17:51 GMT  
		Size: 4.8 MB (4765053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a960e13341a49318f499be6c03e865403f941af98f4357457356c71e939f307`  
		Last Modified: Thu, 18 Jun 2020 21:26:54 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2372a3211da53d466e7b49c856947d71b09a77f5661fc1da11bd38481714f1`  
		Last Modified: Thu, 18 Jun 2020 21:26:54 GMT  
		Size: 323.8 KB (323802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8145f06664e9d6b40af2d07b70b3a8384ae28e3154db12ae5c75a5a8d61fc03c`  
		Last Modified: Mon, 22 Jun 2020 19:30:46 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a0a2b6b5dc61e0666549c20b1b19cf2d3a763012ba6bc2a6a3ebb6b93512e2`  
		Last Modified: Mon, 22 Jun 2020 19:30:47 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc5f18ceec3defcddc313456a25f22107e67a61aefbeef872fe5f94116f4bd9`  
		Last Modified: Mon, 22 Jun 2020 19:30:48 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f643dd45d1af273aecd4224e58e5cf7e5a36daa5670383a8bc3843536b59fd`  
		Last Modified: Mon, 22 Jun 2020 19:31:05 GMT  
		Size: 191.7 MB (191716102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415be66fe740ecb63801054174269690f807019b3a10e07729fd3caed0d4578f`  
		Last Modified: Mon, 22 Jun 2020 19:30:46 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
