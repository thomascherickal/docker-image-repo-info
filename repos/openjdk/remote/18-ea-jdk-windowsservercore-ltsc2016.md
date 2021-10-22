## `openjdk:18-ea-jdk-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:5afe6a0b23b5e195b31d64134f4fed8a3280e64cf7dd6037321ca2e5053ecaed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `openjdk:18-ea-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull openjdk@sha256:1f91c96ff692403f32a1538da2b56bcce64ffbf2dbc73a9f61d26b661eb9462d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6457080013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be909225a44716402e21838211a47855020afaac7c8ae1a1412d48948e03c56e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 12:40:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 00:35:32 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 00:35:33 GMT
ENV JAVA_HOME=C:\openjdk-18
# Thu, 14 Oct 2021 00:36:39 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 21 Oct 2021 23:17:31 GMT
ENV JAVA_VERSION=18-ea+20
# Thu, 21 Oct 2021 23:17:33 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_windows-x64_bin.zip
# Thu, 21 Oct 2021 23:17:34 GMT
ENV JAVA_SHA256=9a0adb8304f31d0e05a1d4a2d848e989e8c195027ef954afdb789977285287e8
# Thu, 21 Oct 2021 23:20:13 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 21 Oct 2021 23:20:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6974b1bd85ba3f9ce16d86231eced43f720fed9c13411d37584dfe7193bcde60`  
		Last Modified: Wed, 13 Oct 2021 13:27:57 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df06f60babff5e4f22bec0a3230e7cb06b975eee8a07f9541607a63c6f54ec1`  
		Last Modified: Sat, 16 Oct 2021 00:35:57 GMT  
		Size: 352.3 KB (352290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d102eb2191e4f3dc1d3161448876d7ca39ddbdf59ce99128c02345b2f37d5a7`  
		Last Modified: Sat, 16 Oct 2021 00:35:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925804b8e49990f4d1d67406a2478bccf5a1d14fc5af2bd05ff3cd31251cf4af`  
		Last Modified: Sat, 16 Oct 2021 00:35:56 GMT  
		Size: 348.2 KB (348170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07eec718139df56546b6dc37b35e193faf655f940599042b7a5a68784d0307fd`  
		Last Modified: Thu, 21 Oct 2021 23:42:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df9b23f855e4264023a33dcedce69306a9e8139114f3adcf8c7531207a6aa1e`  
		Last Modified: Thu, 21 Oct 2021 23:42:57 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b32b483ea3de9cd266e6f7e55bda1786b5d5a27584d4a932bad9c49a857d31f`  
		Last Modified: Thu, 21 Oct 2021 23:42:57 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529271642eb87d754403a299bd8241a213f9c99e981ee57f7b98ff9440993d51`  
		Last Modified: Thu, 21 Oct 2021 23:43:18 GMT  
		Size: 183.6 MB (183604618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9fef5d0ca11637496fac500d0c754939ef2f8dcee6a619eb19aac7fea215ab`  
		Last Modified: Thu, 21 Oct 2021 23:42:57 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
