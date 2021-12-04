## `openjdk:18-ea-jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:a54874b44b252b8e1e4d7c446c1aeb53ca566e5b96f3e9c2cb2e0575a4b646f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.350; amd64

### `openjdk:18-ea-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.350; amd64

```console
$ docker pull openjdk@sha256:090e62f58c60a4bea679118a55cc77c4f54bf0a0f98b9f79bc56abaa7d12612f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2370153666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15aaa551732d2457eb1f135d1773ccfab32811b9701d5a881406c4b97cf0275`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 03 Nov 2021 08:36:33 GMT
RUN Install update ltsc2022-amd64
# Wed, 10 Nov 2021 01:38:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:23:23 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 10 Nov 2021 20:23:24 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 10 Nov 2021 20:23:41 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 03 Dec 2021 23:08:23 GMT
ENV JAVA_VERSION=18-ea+26
# Fri, 03 Dec 2021 23:08:24 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/26/GPL/openjdk-18-ea+26_windows-x64_bin.zip
# Fri, 03 Dec 2021 23:08:24 GMT
ENV JAVA_SHA256=ca0f08726d07f4f0514c35b0e30268cf229e8564aceab51d288f237a5ea9b309
# Fri, 03 Dec 2021 23:09:24 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 03 Dec 2021 23:09:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0eb404f1860fa8786ad09d1d9fe9fd580115f83cd38623bc4eb0c46abdaa0a3`  
		Size: 932.9 MB (932907933 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:27ded59d7006d9d7bffa7c253cd04a900a5d6b0d47b84d0edd624d12fd64cdc9`  
		Last Modified: Wed, 10 Nov 2021 02:07:39 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc4afb60e31b5cebc49ca0785c802982ffcb26a35cbf45cb86cfacf57f997ea`  
		Last Modified: Wed, 10 Nov 2021 21:03:27 GMT  
		Size: 616.5 KB (616541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db941a11fe2589a4b4de4126a25fa46cf249f4a92b8a2096088b8a6ef786873`  
		Last Modified: Wed, 10 Nov 2021 21:03:27 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d59e6a5010c5f473824d430525059a4a652ec50176e6bc1e1b6b1cad7c7a562`  
		Last Modified: Wed, 10 Nov 2021 21:03:27 GMT  
		Size: 549.7 KB (549708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca8b30d9429c155f3579268642beb9360f49c710f758d48460807ea73867cc0`  
		Last Modified: Fri, 03 Dec 2021 23:27:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abcaecac913427e82fceb4be4bc90300676ef5bcab1d36ffed91e2de9936571`  
		Last Modified: Fri, 03 Dec 2021 23:27:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395124962c297ac7179a8e1707e122c6c71ba59aae8d277bbfa55d7fa59f3a30`  
		Last Modified: Fri, 03 Dec 2021 23:27:01 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cc2a32df7254c8d0488734cbfc4773ae236611e53f0f900fc62e03dd8da8e9`  
		Last Modified: Fri, 03 Dec 2021 23:30:21 GMT  
		Size: 184.4 MB (184371957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c714a60c2ea3794542e24d79003f9b4ba5a49ce689827edd7221bd0ff209f9`  
		Last Modified: Fri, 03 Dec 2021 23:27:01 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
