## `openjdk:21-ea-8-windowsservercore`

```console
$ docker pull openjdk@sha256:0d3862dba72c7fd6192a6baf34b9e70620119108d6ce62e61fbef704cbac37cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1487; amd64
	-	windows version 10.0.17763.3887; amd64

### `openjdk:21-ea-8-windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull openjdk@sha256:6e2e3c51a6c9e07c19173b1cc0bae4340a616f0ad0d58ac559594ff273ac8cea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1581909954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c24f757f7099f10f4be1801c39458a378d4c62acf0364073385a399b0dddac84`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:07:34 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 12 Jan 2023 05:07:35 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 12 Jan 2023 05:07:57 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 02 Feb 2023 23:23:13 GMT
ENV JAVA_VERSION=21-ea+8
# Thu, 02 Feb 2023 23:23:14 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_windows-x64_bin.zip
# Thu, 02 Feb 2023 23:23:15 GMT
ENV JAVA_SHA256=3fda88db8f695db1f63db79299e59eaaa3733bad3a5e46677af1c97992fbc3f1
# Thu, 02 Feb 2023 23:24:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 02 Feb 2023 23:24:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa8e5b91e3c425a756945d0dec251c1595992592fd0dcf4df0ec0a7962717eb`  
		Last Modified: Thu, 12 Jan 2023 05:22:24 GMT  
		Size: 614.6 KB (614563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6284573ed998f0926754c8fd5dc7faff95102e54cf06b0d280cd07428b048e11`  
		Last Modified: Thu, 12 Jan 2023 05:22:23 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee2720203565dd5e40979d2f76187379d7c05254dd58609d0f974f653b1db40`  
		Last Modified: Thu, 12 Jan 2023 05:22:24 GMT  
		Size: 552.5 KB (552462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a40494a3af0aaf963a61a8b5bf6f3b333f54350715a6d87a61aa774a7602c6`  
		Last Modified: Fri, 03 Feb 2023 00:23:40 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da258df90edf0588436046378964ef1ece52f5ccd3e0132800a286cdbbf2447`  
		Last Modified: Fri, 03 Feb 2023 00:23:40 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4632c630bdc6bc41cc21c761dd6c6def18f8d7243e5a3aff1e43d6ef8fd8fce6`  
		Last Modified: Fri, 03 Feb 2023 00:23:40 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8f1b8a3277453e9ec81dcdcbfd8618860fe09aa0e31d1e5cbf7844fcefa9fc`  
		Last Modified: Fri, 03 Feb 2023 00:24:03 GMT  
		Size: 194.7 MB (194705381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a03fc1566ed1c502c86b5ff90ea15c557197b782430a10d0033ad07bcfa9fbf`  
		Last Modified: Fri, 03 Feb 2023 00:23:40 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-8-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull openjdk@sha256:54177cb47cd6cf5626a99571629938eb78793caabf62c0270f8de12ddd3cbaae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1903136758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c42bc6e83910b3191002e7cf4baf52be607e6cd0a180ac7e9bbd977cfcefc29`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:09:35 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 12 Jan 2023 05:09:36 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 12 Jan 2023 05:10:00 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 02 Feb 2023 23:24:30 GMT
ENV JAVA_VERSION=21-ea+8
# Thu, 02 Feb 2023 23:24:32 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk21/8/GPL/openjdk-21-ea+8_windows-x64_bin.zip
# Thu, 02 Feb 2023 23:24:33 GMT
ENV JAVA_SHA256=3fda88db8f695db1f63db79299e59eaaa3733bad3a5e46677af1c97992fbc3f1
# Thu, 02 Feb 2023 23:25:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 02 Feb 2023 23:25:52 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fe1d317f0927d209417077d671ba0fb8e3b7ff9c583727da819f0d16252e80`  
		Last Modified: Thu, 12 Jan 2023 05:23:04 GMT  
		Size: 367.5 KB (367453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6807e3d75deac242f3cfe460728c148c2f68e1d8366ad3f0358a3c9237042b6`  
		Last Modified: Thu, 12 Jan 2023 05:23:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbe0b64cf9fa2560a38a4c1a75582463f16f8e35e9776b14d87cd13167e4281`  
		Last Modified: Thu, 12 Jan 2023 05:23:04 GMT  
		Size: 320.0 KB (320032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7c4390b29dd1012cda10021de29bf2d7417d7264842d047565aa337c9da6e3`  
		Last Modified: Fri, 03 Feb 2023 00:24:22 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d57f118dffdef8dc7d1890e376dc69c8894f02bff381f0110a571b6eec22ed5`  
		Last Modified: Fri, 03 Feb 2023 00:24:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3701656fd7cff8d412506aebeba1667a45831cf2690c9258993c9c054db81b50`  
		Last Modified: Fri, 03 Feb 2023 00:24:22 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7f9545fe8974838c64e16caa088af3b2ce18c50f46f74062207644a3220322`  
		Last Modified: Fri, 03 Feb 2023 00:24:44 GMT  
		Size: 194.5 MB (194496900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1763ab6e89ab93f6b7227ad4b8cf48ff4cae49201961cc0d40f432340a78ab22`  
		Last Modified: Fri, 03 Feb 2023 00:24:22 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
