## `eclipse-temurin:17-jre-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:856355ce70e628535e2d7a08f4cb0043b4513758e44587051481f8de8c9891c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:17-jre-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:16f851b07a37d10d2fd2d7cc9e73cdc0a1f612dfbbcaac6b2e0549b8630e53cb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2790745172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7069042a559b3d32170a6b73aec0ee2a1a4afcc07ac3eb6b5f44e7d758c816d0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 19:29:54 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 26 Jan 2022 19:38:07 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_x64_windows_hotspot_17.0.1_12.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_x64_windows_hotspot_17.0.1_12.msi ;     Write-Host ('Verifying sha256 (f1580b6aa2071448798d5f5e3c229fc150cb5bc4e650c365121be9afdf4c313b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f1580b6aa2071448798d5f5e3c229fc150cb5bc4e650c365121be9afdf4c313b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 26 Jan 2022 19:39:14 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773f4e699349765fd45db03b2449262203789f6bfaf2feed85f734ba7530b162`  
		Last Modified: Wed, 26 Jan 2022 20:16:35 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cfb1a2034e09bcf422cec623c4a3d07914e500305643430231f1e42bc1f33b`  
		Last Modified: Wed, 26 Jan 2022 20:24:23 GMT  
		Size: 74.1 MB (74142816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed440a0d95781ec2d0e6bcfb56cb35765d98cec6a237d20b1a01e16ac096a93b`  
		Last Modified: Wed, 26 Jan 2022 20:22:56 GMT  
		Size: 3.3 MB (3278028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
