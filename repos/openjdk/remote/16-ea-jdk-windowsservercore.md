## `openjdk:16-ea-jdk-windowsservercore`

```console
$ docker pull openjdk@sha256:e247f540c657a72997b41451234e6b5e8e1ccdbff0d76e5faf890bef59784828
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64
	-	windows version 10.0.14393.3808; amd64

### `openjdk:16-ea-jdk-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:bb5f6f1f8e2b9693391feea7ad9b2b09e5ed1b0290ff277b454764beba81d611
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2516366028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f96d481a2293b55dad0a416bf10a59949151e506d345091e6a6c7e878788079`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 24 Jul 2020 18:15:15 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Fri, 24 Jul 2020 18:15:17 GMT
ENV JAVA_HOME=C:\openjdk-16
# Fri, 24 Jul 2020 18:15:38 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Fri, 24 Jul 2020 18:15:39 GMT
ENV JAVA_VERSION=16-ea+7
# Fri, 24 Jul 2020 18:15:40 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/7/GPL/openjdk-16-ea+7_windows-x64_bin.zip
# Fri, 24 Jul 2020 18:15:41 GMT
ENV JAVA_SHA256=51f0d39c14feb7c4ce970aebb3ec35c33b6511023842c1122c62b83ea3292339
# Fri, 24 Jul 2020 18:17:36 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 24 Jul 2020 18:17:38 GMT
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
	-	`sha256:0ded26bb196400f1cf541826f3f44c1025664089ba3c58aaf3b7afca018655df`  
		Last Modified: Fri, 24 Jul 2020 18:33:13 GMT  
		Size: 9.2 MB (9158926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5331aed97b004095fa939fcf32a60be450a462a6f710beea77b4507e4416fe`  
		Last Modified: Fri, 24 Jul 2020 18:33:10 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a58fddb23ea3a144374036b7f928eae28c094b087ba205a4baf4682fa25526`  
		Last Modified: Fri, 24 Jul 2020 18:33:10 GMT  
		Size: 314.1 KB (314142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040d8e7b6bbcaa8fe9decd8506d9d718e274845544a74b772200554dfc06d565`  
		Last Modified: Fri, 24 Jul 2020 18:33:07 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0606679a8e3060ab4af4a10762769adf8af071ea395181b2d9820bb0b602e4`  
		Last Modified: Fri, 24 Jul 2020 18:33:07 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27af739d03a2f327b178e8c6da27e7051f82c658357e89798db52b9d479af9b0`  
		Last Modified: Fri, 24 Jul 2020 18:33:07 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d96a6c98c2dbd145a41141ac99be14e691f993eb1e4dc1df1cc626333ab379`  
		Last Modified: Fri, 24 Jul 2020 18:33:31 GMT  
		Size: 196.7 MB (196694057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41bd10864cf9bf90fcd0a495337be90cb439d9ebcdcbcc15cca4e4e49bc7167f`  
		Last Modified: Fri, 24 Jul 2020 18:33:07 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-ea-jdk-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull openjdk@sha256:a67654a4c96fea751fd8ed59232c4437afc8a486de7b2f8aa446daed62fa0d18
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5954523630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe224004378767d0f831b22756c34c9061d29f01f9be1abb1caae0973060640d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 21 Jul 2020 16:57:52 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Tue, 21 Jul 2020 16:57:54 GMT
ENV JAVA_HOME=C:\openjdk-16
# Tue, 21 Jul 2020 17:02:33 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Fri, 24 Jul 2020 18:17:48 GMT
ENV JAVA_VERSION=16-ea+7
# Fri, 24 Jul 2020 18:17:49 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/7/GPL/openjdk-16-ea+7_windows-x64_bin.zip
# Fri, 24 Jul 2020 18:17:50 GMT
ENV JAVA_SHA256=51f0d39c14feb7c4ce970aebb3ec35c33b6511023842c1122c62b83ea3292339
# Fri, 24 Jul 2020 18:20:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 24 Jul 2020 18:20:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecf5cd76cb63f861b644ea8339d6249d5372f121099524df379003e1bbb30d9`  
		Last Modified: Tue, 21 Jul 2020 17:37:06 GMT  
		Size: 9.9 MB (9859351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63530cffa1eb60604458a400041ef9cbdb94004186de71aa32a3a4bc08e8561d`  
		Last Modified: Tue, 21 Jul 2020 17:37:03 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfeb8a5d9ef6f3cada7404d604fb88f291e3e4ab57b78ebe38a6f9733d83881d`  
		Last Modified: Tue, 21 Jul 2020 17:37:06 GMT  
		Size: 5.4 MB (5366955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3df0bde0fa6ac282c415eb0ca28281f90d4151f801b077cddcd794936f367a5`  
		Last Modified: Fri, 24 Jul 2020 18:33:52 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799b082a48aa715291c3aefe88bf370fc8591537eacc8f2051c3f068ef282132`  
		Last Modified: Fri, 24 Jul 2020 18:33:52 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73748772021f02f1cfae40318066266367ecb785946a2f8f1fb59dbeb39c739`  
		Last Modified: Fri, 24 Jul 2020 18:33:51 GMT  
		Size: 1.1 KB (1108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b502bf70eb0ea692ca035cf1f10d3f2b3b32b7b80a8c213d69c8d8a99a60a875`  
		Last Modified: Fri, 24 Jul 2020 18:34:14 GMT  
		Size: 201.8 MB (201828559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90675affc0a1f191941f29cf1998efe97920c1433c6746aed58b00a2d13e8591`  
		Last Modified: Fri, 24 Jul 2020 18:33:52 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
