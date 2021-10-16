## `openjdk:jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:15ef0fdf78671d7ec61367a1933a6c441ab866e14a6a04b2584c823f6a3054a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `openjdk:jdk-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:d70c484a8ef2d0ba5a457886fb35fa91abb53b3b2e87c2fb97d675a96073afcc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2869409923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1e870e26c50059995795fd88f93303f6510b97a5afe01fdc44935cfe86cf898`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 00:31:04 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 00:39:46 GMT
ENV JAVA_HOME=C:\openjdk-17
# Thu, 14 Oct 2021 00:40:50 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 00:40:51 GMT
ENV JAVA_VERSION=17
# Thu, 14 Oct 2021 00:40:52 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk17/0d483333a00540d886896bac774ff48b/35/GPL/openjdk-17_windows-x64_bin.zip
# Thu, 14 Oct 2021 00:40:53 GMT
ENV JAVA_SHA256=e88b0df00021c9d266bb435c9a95fdc67d1948cce4518daf85c234907bd393c5
# Thu, 14 Oct 2021 00:42:27 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 14 Oct 2021 00:42:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3778f0ab9c363534bcf1068a50329066ca025f6499401dd667a232ffdd9687e4`  
		Last Modified: Sat, 16 Oct 2021 00:35:18 GMT  
		Size: 349.3 KB (349328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a55cdf95057f198bde59030fd87aaaad8a9cce8f2e0224fbcda5c91a7d2f61`  
		Last Modified: Sat, 16 Oct 2021 00:40:15 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328d7ad425f8dc11d681aa24a655c9b82be416ac60ac7c492ee6b6e397fc471e`  
		Last Modified: Sat, 16 Oct 2021 00:40:15 GMT  
		Size: 310.7 KB (310707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e31c361f7f802b88fdc9d7a438da06eb8de1ae38d062fe8a49ec452cfe8d56`  
		Last Modified: Sat, 16 Oct 2021 00:40:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce9b2f2a8e8e7b84a4e60e5124097973f6c12d1e3758b364567ae34f12051cf`  
		Last Modified: Sat, 16 Oct 2021 00:40:12 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c122004605e3c3d5e31212469464f45627d6accbcfd821942f18882265439fac`  
		Last Modified: Sat, 16 Oct 2021 00:40:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dde5ccf6fdbc394147ae1c1dd52964d71ac9d70c124bef5db8fe91d3348acd1`  
		Last Modified: Sat, 16 Oct 2021 00:40:31 GMT  
		Size: 182.4 MB (182422608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2208aa6b8a1e600514a3d00046a22ad748d67d98bec47c17b84ac12ba98a1484`  
		Last Modified: Sat, 16 Oct 2021 00:40:12 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
