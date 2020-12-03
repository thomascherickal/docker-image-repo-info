## `openjdk:16-ea-27-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:060e26b7a256d4c724c3e7816567a8f5d41f66d9f14c6bd43993cf736dd35c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `openjdk:16-ea-27-jdk-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull openjdk@sha256:c77f4eaf2e7d10ddaf703a8709dcc0f9da5de6da2938fe180ba1a4ac899b7a5b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2582322815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b7219759236d976233371cf3375ae367cd556c5577212e92d83de0e5bb801ca`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 17:45:35 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Wed, 11 Nov 2020 17:45:36 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 11 Nov 2020 17:45:58 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Thu, 03 Dec 2020 22:14:16 GMT
ENV JAVA_VERSION=16-ea+27
# Thu, 03 Dec 2020 22:14:17 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk16/27/GPL/openjdk-16-ea+27_windows-x64_bin.zip
# Thu, 03 Dec 2020 22:14:18 GMT
ENV JAVA_SHA256=b2d10f066df03f1b3e5a6f4c319bda1169deb346ebe4b8a98852dbbf678e2f8b
# Thu, 03 Dec 2020 22:15:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 03 Dec 2020 22:15:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bee39b5545a888688525644d5ac139bf90e9e5031cc78ac03612316b125116`  
		Last Modified: Wed, 11 Nov 2020 18:25:54 GMT  
		Size: 9.2 MB (9240273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137fed5035462ef3e8b61dc554137650a8cfdbda487936adb705e2cd184bf115`  
		Last Modified: Wed, 11 Nov 2020 18:25:43 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c03d4f5a3977a1dad2edfe3806bcaa8f0d4ce2d47ea49f0fdc3a58fc019897f`  
		Last Modified: Wed, 11 Nov 2020 18:25:43 GMT  
		Size: 307.0 KB (307020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3daf983ec27783c503afea720496ad8637e8910bd284b7dac93511795e2f4a`  
		Last Modified: Thu, 03 Dec 2020 22:23:27 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd16e6ffb000c027aa6da60be47e489c137019a63ae4856ae004f871c91aa5e`  
		Last Modified: Thu, 03 Dec 2020 22:23:27 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fd4f9cc6864ec1dbd15b02beea72bd2b6666e800d832f46af0c8a91c24d771`  
		Last Modified: Thu, 03 Dec 2020 22:23:27 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c69b53e0aa91067343e8a7cb6b6f88caa69d96f02c8cdaec3711cfeb90ed27f`  
		Last Modified: Thu, 03 Dec 2020 22:23:47 GMT  
		Size: 184.7 MB (184739430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e60d1824096d1e80fa8f999cb6305a3173318c18b5f56dbc92ab5213f24dead`  
		Last Modified: Thu, 03 Dec 2020 22:23:27 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
