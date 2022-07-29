## `openjdk:19-ea-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:a011c27a46bf679cfcc1f4c8954639aca6b210f0c32f213a3591f056d5c8a2de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `openjdk:19-ea-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull openjdk@sha256:e673f910edcc6ae447ee7b9bea3f31995f4215ec9ebc2c7adb52e6a182acce74
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2493211278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d2ae1427b74ccb43bc1a83daeb1d1a4ea1c3da1e5a00546d5e3affccb73aa43`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jul 2022 15:47:47 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 13 Jul 2022 15:53:28 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 13 Jul 2022 15:53:49 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 29 Jul 2022 01:19:52 GMT
ENV JAVA_VERSION=19-ea+33
# Fri, 29 Jul 2022 01:19:53 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/33/GPL/openjdk-19-ea+33_windows-x64_bin.zip
# Fri, 29 Jul 2022 01:19:54 GMT
ENV JAVA_SHA256=5e751d1216c33ba6097545ff14860507a9a5a8d6d1ca482b24280f7104865b2d
# Fri, 29 Jul 2022 01:20:48 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 29 Jul 2022 01:20:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6a9bb0f902c90ab99dd7b3c8634f73649b052868aa5272230088be93b0be1f`  
		Last Modified: Mon, 18 Jul 2022 21:21:07 GMT  
		Size: 655.6 KB (655645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd66eccfd01aee1696d4c33d4a0c1b49827e90518a13fde80169d46f2171f64`  
		Last Modified: Mon, 18 Jul 2022 21:23:16 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a625d17ec9ae423e7fd6a2cd3d934b06c1a4872336d21f5021622a34e145e1`  
		Last Modified: Mon, 18 Jul 2022 21:23:16 GMT  
		Size: 555.8 KB (555849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2dd5ec7d268b3240b385721aa6cb5b0cb15edbcb4cf4ba8355e199e52d9642`  
		Last Modified: Fri, 29 Jul 2022 03:21:56 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d03ecfef5a83e9ba113263862abf10139788feb17b4833f8e4b4e7b8a67a34e`  
		Last Modified: Fri, 29 Jul 2022 03:21:56 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73626b24fea14c56b1135d9e10acb7f07e11089b1a84d426344202b9b744f24`  
		Last Modified: Fri, 29 Jul 2022 03:21:57 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a470278aff5312aaec9e26cea2e930982fe9b19da34bc0229327c3bd2d4d8484`  
		Last Modified: Fri, 29 Jul 2022 03:22:16 GMT  
		Size: 191.8 MB (191760088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde8ec4c84dbd59ec3260c39cc832b08fc2351d4da6157c403e0549e00899461`  
		Last Modified: Fri, 29 Jul 2022 03:21:56 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
