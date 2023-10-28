## `openjdk:22-ea-jdk-windowsservercore-ltsc2022`

```console
$ docker pull openjdk@sha256:277f1f661c1324660ba22b95127808b027f4d5ea32a27aa49761b23b72aea366
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `openjdk:22-ea-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull openjdk@sha256:b718444f3b4cec215c88250100ffa77afe7ed91d4103475c36fb3e1a044587cd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2060277467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15b3617b0f476a77591f6a664ef8952c0f4ab62a5d2db8aeeaf770ead3819ed`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 03:48:56 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 11 Oct 2023 03:48:57 GMT
ENV JAVA_HOME=C:\openjdk-22
# Wed, 11 Oct 2023 03:49:19 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 28 Oct 2023 01:15:01 GMT
ENV JAVA_VERSION=22-ea+21
# Sat, 28 Oct 2023 01:15:02 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_windows-x64_bin.zip
# Sat, 28 Oct 2023 01:15:03 GMT
ENV JAVA_SHA256=afd96ebc47e8681ed848af5055604a81fc4d42b0153541923f3cc49fd0eb36fb
# Sat, 28 Oct 2023 01:15:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 28 Oct 2023 01:15:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71221770428be33fb112dc7596eb2857d0a894b9444c8ac1e070fb2713cf0cef`  
		Last Modified: Wed, 11 Oct 2023 03:55:46 GMT  
		Size: 438.1 KB (438050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7edf8e3cbf42462ac6609acad01b5456938cdcc07b096dfebda103810e262f`  
		Last Modified: Wed, 11 Oct 2023 03:55:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935ab285e7bf5c8a65c15bf37e24c811dc80f14c18753ee554d67b2924e05265`  
		Last Modified: Wed, 11 Oct 2023 03:55:45 GMT  
		Size: 251.8 KB (251804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cead219de823db0c49212d4cfed097e5226f4327a1226eb5de6c488f6ee029e`  
		Last Modified: Sat, 28 Oct 2023 01:18:52 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6214b5372aaa925299e06bd9acca1d95be5fc8db11a051e4606e035306d99720`  
		Last Modified: Sat, 28 Oct 2023 01:18:52 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691a3d68bda27e78dc79437c60b78d33415460f3731a9976f0abe96d4b960481`  
		Last Modified: Sat, 28 Oct 2023 01:18:52 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b8227f0c954638caffe158fa7576c6ceefa4ae1e3db91f2de2d2fb40ee32f7`  
		Last Modified: Sat, 28 Oct 2023 01:19:10 GMT  
		Size: 199.7 MB (199736188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ad8854c6b834dd1f528f30784ba877df178a5969f69d62097bbcecd41632f4`  
		Last Modified: Sat, 28 Oct 2023 01:18:52 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
