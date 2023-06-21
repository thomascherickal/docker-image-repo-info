## `openjdk:22-jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:6eefc13fac1a19cd44820314d19ff58fd7971bcee77a43c9ef70af55cfc6b989
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `openjdk:22-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull openjdk@sha256:3e05b9eef3718566160b7a33eb36b4cc9d9494e2de48475964310d7ab42a23fd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.6 GB (1588202113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d22041872309c0c69c170785f68479d008604fa906afd1c1bbd8f27fef7e0d8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 17:38:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 20:24:17 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Jun 2023 20:24:18 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 14 Jun 2023 20:24:40 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 21 Jun 2023 01:53:56 GMT
ENV JAVA_VERSION=22-ea+2
# Wed, 21 Jun 2023 01:53:57 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/2/GPL/openjdk-22-ea+2_windows-x64_bin.zip
# Wed, 21 Jun 2023 01:53:58 GMT
ENV JAVA_SHA256=5c387014bc480e9bc3e204504d0fcd933912694e6a4a44c044696e4f2a9b7ca1
# Wed, 21 Jun 2023 01:54:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 21 Jun 2023 01:54:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972ddd233121a2afd2cf1a3eaec49d595cfe6b3ebe19ef3dd492d99784c370f`  
		Last Modified: Wed, 14 Jun 2023 18:17:55 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ecf7cfdecc4064a3b0d43346d08171233c7f384d58889a6b8710f45b5c57a9`  
		Last Modified: Wed, 14 Jun 2023 20:33:59 GMT  
		Size: 318.3 KB (318286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9624736e3a137e1fc18ba10e5204d02182493f45248b8244fd30cb115ab166da`  
		Last Modified: Wed, 14 Jun 2023 20:33:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5471f5a4ff982cd1b1f54bc26a1c71ee3ff0a92a312f7bb6e09d5021cf7f39`  
		Last Modified: Wed, 14 Jun 2023 20:33:59 GMT  
		Size: 263.1 KB (263055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cf31a809430d76e94a07cc072ef789523bfbc46f90c6e99fb6a148c4aa9e3b`  
		Last Modified: Wed, 21 Jun 2023 02:01:01 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2628f4e0cf90272caa6b9d3fb48f911a35db7b82b51d00154146ef2b408d900b`  
		Last Modified: Wed, 21 Jun 2023 02:01:01 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e933804681f0a8072a9f6baef482214040b108fc1dbd753d6b4d7483ee97f831`  
		Last Modified: Wed, 21 Jun 2023 02:01:01 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b3fef6f6e66fc1f2b6fea916cf0d81bcaa6c7cd24a5b26cda47a7e41f6bd11`  
		Last Modified: Wed, 21 Jun 2023 02:01:23 GMT  
		Size: 199.0 MB (199014213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f51a81262768b30e44b52d44a2e39c71b8d319a5d3bafaf07dfb623b8fb5962`  
		Last Modified: Wed, 21 Jun 2023 02:01:01 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
