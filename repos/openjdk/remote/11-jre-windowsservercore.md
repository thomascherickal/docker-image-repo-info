## `openjdk:11-jre-windowsservercore`

```console
$ docker pull openjdk@sha256:d5665303e4f98798d6b34cd70a5058120151fe5408f6fad7a8ad3f004590dfad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.643; amd64
	-	windows version 10.0.17763.2803; amd64

### `openjdk:11-jre-windowsservercore` - windows version 10.0.20348.643; amd64

```console
$ docker pull openjdk@sha256:38ac9adc7ea886db3a94097e3168a4d82b3a6604b5b1dd57e82cb21ab9ed94e0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2268204721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:751e3c5bb97e3580594272a078cf734f69c16c46245cb9c47ada10e98733f0ad`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 16:55:44 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Apr 2022 17:11:01 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 Apr 2022 17:11:23 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 25 Apr 2022 18:27:39 GMT
ENV JAVA_VERSION=11.0.15
# Mon, 25 Apr 2022 18:31:05 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11u-jre_x64_windows_11.0.15_10.zip
# Mon, 25 Apr 2022 18:31:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c156288a763e09322f37d1214a5fcfaa1ebfbf8a108ee1351f5321537e137ef`  
		Last Modified: Tue, 19 Apr 2022 00:49:30 GMT  
		Size: 629.6 KB (629633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14570f98afbbd26047ba4240c4fbc7d318dafb1305f4fc74ff47a6d56ddf8db7`  
		Last Modified: Tue, 19 Apr 2022 01:07:05 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a921e6feaf37907e9ca9b3b20d208d4a385093b5a66da6c8f9f7e2330057813`  
		Last Modified: Tue, 19 Apr 2022 01:07:03 GMT  
		Size: 559.9 KB (559854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab36691fd2a01c0d96f08be815d7b18dc6f6820a153eb4bf1b5bf06411051910`  
		Last Modified: Mon, 25 Apr 2022 20:29:48 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac4cd395bbca27f823701889395d5a972f6a80673003458d08b308330081d2b`  
		Last Modified: Mon, 25 Apr 2022 20:34:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9d56e74b4206732d4e65c847ce234e159b7398a31d46af9213da7bdc294c7a`  
		Last Modified: Mon, 25 Apr 2022 20:35:45 GMT  
		Size: 40.1 MB (40054788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:11-jre-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull openjdk@sha256:618b61e180ce6401b751d20feb5cb9a435d49dc5991438be3321ddf5cf983002
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2756426092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0732c22d3c18b70aecaead6b1c11f7cda44d2edc25f19d33fd58b106b5ba4b23`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 13 Apr 2022 17:12:29 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 Apr 2022 17:13:21 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Mon, 25 Apr 2022 18:28:42 GMT
ENV JAVA_VERSION=11.0.15
# Mon, 25 Apr 2022 18:31:57 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11u-jre_x64_windows_11.0.15_10.zip
# Mon, 25 Apr 2022 18:33:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
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
	-	`sha256:b6192cb36d606379e184b63db7af3a89f4810b2f64e5800fd6e420b40ffabf19`  
		Last Modified: Tue, 19 Apr 2022 01:07:48 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdbb07a3938aad3dd6d9776f20503fe1ac793e4c8c244ea54dbbb2a55298c0d`  
		Last Modified: Tue, 19 Apr 2022 01:07:46 GMT  
		Size: 322.2 KB (322215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26bf718182608fab7eafc9f4a299dadadfb51d4429660902b23a859dfab5fa5`  
		Last Modified: Mon, 25 Apr 2022 20:30:27 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c9fb4bcdbcd195056a013b9b158a5f56e28d9bee95f57612673986c5585fed`  
		Last Modified: Mon, 25 Apr 2022 20:35:57 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4053a8bc14288ebd9ddf39b4b9c3d0ab2bf176624d9fd97d2c2e0bc19ed5a`  
		Last Modified: Mon, 25 Apr 2022 20:36:04 GMT  
		Size: 39.8 MB (39811337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
