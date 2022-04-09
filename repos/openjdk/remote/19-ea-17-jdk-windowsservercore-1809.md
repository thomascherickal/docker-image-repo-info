## `openjdk:19-ea-17-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:d7a09b75167b368b47c333bc27de746995e7636b7e197d40f78cde4318f4644b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `openjdk:19-ea-17-jdk-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull openjdk@sha256:e3585d60217c559422d74925e3416c37207ac2533ff023f75063d47d11a82c2d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2905282422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d47f2a8aa7e90ef51c4f6e3b15ed084286879129107305200898870eaca53f54`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 17:11:03 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 09 Mar 2022 17:11:04 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 09 Mar 2022 17:11:56 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 08 Apr 2022 20:17:05 GMT
ENV JAVA_VERSION=19-ea+17
# Fri, 08 Apr 2022 20:17:06 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk19/17/GPL/openjdk-19-ea+17_windows-x64_bin.zip
# Fri, 08 Apr 2022 20:17:07 GMT
ENV JAVA_SHA256=30beef80c4735aeac527ee2665455ea07b3f1885d501f949e500882d6dc6b898
# Fri, 08 Apr 2022 20:19:01 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 08 Apr 2022 20:19:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082ea46951b109a477871d3f8739d105427abdbef68b50e54b54b4ed440f48e8`  
		Last Modified: Wed, 09 Mar 2022 17:41:38 GMT  
		Size: 356.5 KB (356505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c303714362d4354175bfbd60bde4487fb5663326536432755fabbeca5237db`  
		Last Modified: Wed, 09 Mar 2022 17:41:37 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ced75f82f0e7f243af02f1c1abe1b9baafcfd9b31f208d60f85f675e0fb5c1`  
		Last Modified: Wed, 09 Mar 2022 17:41:37 GMT  
		Size: 310.2 KB (310174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a7ce032c9ab34e3b516c50fe7084f4eb0e8422fcf368d70285b22b1639ab01`  
		Last Modified: Fri, 08 Apr 2022 23:24:03 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f12a378c48de3966c02795e44af6e3899188d3861258c7958c94fb79b0246a`  
		Last Modified: Fri, 08 Apr 2022 23:24:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5743d546579d9b8e6c3e52fdfb80c269fa8cf376443e63d94bb5ed0c12ad76`  
		Last Modified: Fri, 08 Apr 2022 23:24:03 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3038b35a39bb224b353de619e79e6afacaea42f78601b0b3683acf04fcbc5ef`  
		Last Modified: Fri, 08 Apr 2022 23:24:27 GMT  
		Size: 189.2 MB (189154742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8404657b5780d8186ae54cf6fd6e4f7ca3cef73be44f57b6d8d8e0328a836ae9`  
		Last Modified: Fri, 08 Apr 2022 23:24:03 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
