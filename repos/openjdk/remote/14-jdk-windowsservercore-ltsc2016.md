## `openjdk:14-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:f78a9ba1c28db3d2bbdbc78dc469658738696aacc6bad1f020c1afd0768f5e54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `openjdk:14-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull openjdk@sha256:3dc9db3c86326f256595d5cd2cee44982e42aaa1dc3f82ddd2a3da4ac5bd3835
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5938139559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:623af4687ae2f129c21720af4ad6bc7921f3f771a989a8f88eea9fe9e0df3007`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 14 Apr 2020 21:37:12 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Tue, 14 Apr 2020 21:46:23 GMT
ENV JAVA_HOME=C:\openjdk-14
# Tue, 14 Apr 2020 21:47:40 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 14 Apr 2020 21:47:41 GMT
ENV JAVA_VERSION=14.0.1
# Tue, 14 Apr 2020 21:47:42 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk14.0.1/664493ef4a6946b186ff29eb326336a2/7/GPL/openjdk-14.0.1_windows-x64_bin.zip
# Tue, 14 Apr 2020 21:47:43 GMT
ENV JAVA_SHA256=26255f3f2fe7168ec0dce9d9f3825649c18540ba86279a7506c7f17dd3e537f9
# Tue, 14 Apr 2020 21:50:12 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 14 Apr 2020 21:50:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7792b001970c03ccacbdc7259d0133f320d88e7fdd9394b9c70fe73808fe3ca`  
		Last Modified: Tue, 14 Apr 2020 22:16:39 GMT  
		Size: 5.4 MB (5386185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77477ba8b91a77a67431847f298e15f0baff0be51605640dc4e37db3b776c96f`  
		Last Modified: Tue, 14 Apr 2020 22:18:46 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3ed5c2f97b160b63e3ab61197c7df1aef7bd3be98eeff5092d44fb3e87863e`  
		Last Modified: Tue, 14 Apr 2020 22:18:48 GMT  
		Size: 5.4 MB (5366459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f766211817d0a69b0e71fb8ca09b602726185b43198c86dac91040ed1dced2e8`  
		Last Modified: Tue, 14 Apr 2020 22:18:43 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f11cc864ddfc07333853a5cb4ae4725d97b2102efde386e361e0eced0787ae`  
		Last Modified: Tue, 14 Apr 2020 22:18:43 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12504050dbfae8a261035fd160e9ff4f5be8d396c5ee746451131e54177ae5e7`  
		Last Modified: Tue, 14 Apr 2020 22:18:43 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ed02bbcc30fd8c45ff4679b093b474a7db67d83f5c5e7efa0cd56b8b27c2d1`  
		Last Modified: Tue, 14 Apr 2020 22:19:05 GMT  
		Size: 199.3 MB (199312490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3da32b450a297bc022c62ca6cc782801c9d711f0be3c18e0f82da22d417255`  
		Last Modified: Tue, 14 Apr 2020 22:18:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
