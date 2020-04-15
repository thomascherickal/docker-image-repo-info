## `openjdk:14-jdk-windowsservercore`

```console
$ docker pull openjdk@sha256:5eb5e0a29b982e7bdbc1a28c2bc752bf3be843943c7570ac5f2eacb320920b57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64
	-	windows version 10.0.14393.3630; amd64

### `openjdk:14-jdk-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull openjdk@sha256:1c3fc36f9267f04745d330df6d516cf8fd6d290c84621f7eaa27e29adc0a1fa5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2469949202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc24c8576e1d06d1456d661fcc72bbf54d354e30e054e06122cc1f7b96ce2237`
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
# Tue, 14 Apr 2020 21:44:06 GMT
ENV JAVA_HOME=C:\openjdk-14
# Tue, 14 Apr 2020 21:44:29 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Tue, 14 Apr 2020 21:44:30 GMT
ENV JAVA_VERSION=14.0.1
# Tue, 14 Apr 2020 21:44:31 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk14.0.1/664493ef4a6946b186ff29eb326336a2/7/GPL/openjdk-14.0.1_windows-x64_bin.zip
# Tue, 14 Apr 2020 21:44:32 GMT
ENV JAVA_SHA256=26255f3f2fe7168ec0dce9d9f3825649c18540ba86279a7506c7f17dd3e537f9
# Tue, 14 Apr 2020 21:46:10 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Tue, 14 Apr 2020 21:46:13 GMT
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
	-	`sha256:0aa07c412ac0e934a6b4be075ca0c8af6ac693fa0d9bc2f5f7dc9a5cc9be7d44`  
		Last Modified: Tue, 14 Apr 2020 22:18:00 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7220c68f028be88915f85f89e5e61c28225a04abcbde96c4632c189fe101d01a`  
		Last Modified: Tue, 14 Apr 2020 22:18:00 GMT  
		Size: 296.0 KB (295996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e24a3c1f73d7db8e3720cdb6c87312328aba7caec453ca53f9f60a14b91dd`  
		Last Modified: Tue, 14 Apr 2020 22:17:57 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50e8ced2a3cdc51e62e578ba96e4b719107efd5b9bac16f490016251be57816`  
		Last Modified: Tue, 14 Apr 2020 22:17:57 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59ee36adbd5bf4b4828262ca96ead9ca81f4659bb91cf8293c1a43f3820140e`  
		Last Modified: Tue, 14 Apr 2020 22:17:57 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cac1c8e47b1c20c67071d4c2e212725abc8701fcbd5e969789f9b860dd13d4`  
		Last Modified: Tue, 14 Apr 2020 22:18:17 GMT  
		Size: 194.3 MB (194268624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd025338cf0978d0ed1b68f5d2db1170212ac831cbda4c7a30abf91a454cbf2`  
		Last Modified: Tue, 14 Apr 2020 22:17:57 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:14-jdk-windowsservercore` - windows version 10.0.14393.3630; amd64

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
