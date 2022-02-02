## `eclipse-temurin:11-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:a4ef2459c88aae1fc54e1486be03d35ce8ee032d6661d760bf2c491e3e600f99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.473; amd64
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:11-windowsservercore` - windows version 10.0.20348.473; amd64

```console
$ docker pull eclipse-temurin@sha256:14db8a4574d1deff831b8900f2dfbc7babf065eda93524e8fbffc190e4f689a7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2574243306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf15b499639d02c5150f590d29e60020549a341e1b3075ca1071e4b477c3633`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 16 Jan 2022 05:17:24 GMT
RUN Install update ltsc2022-amd64
# Wed, 19 Jan 2022 22:21:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Feb 2022 22:26:11 GMT
ENV JAVA_VERSION=jdk-11.0.14+9
# Tue, 01 Feb 2022 22:27:49 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.14_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.14_9.msi ;     Write-Host ('Verifying sha256 (067ff937c3220c5c5fc5c75d82061e99dd6f60d50561c565d231670a8b5e510b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '067ff937c3220c5c5fc5c75d82061e99dd6f60d50561c565d231670a8b5e510b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Tue, 01 Feb 2022 22:28:12 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Tue, 01 Feb 2022 22:28:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0e02c12b1310e6c76c29fcd6f81905400fdb6a01caac9dc825939ad004baffef`  
		Size: 955.8 MB (955800778 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2e1f45a873642f0aab3474828d75469362741244e7c714068ac1afe056102cd6`  
		Last Modified: Thu, 20 Jan 2022 00:40:19 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d7056f32c935767c55e432e2b391bd2c63ca5f09282c611b20b0c3d6704103`  
		Last Modified: Wed, 02 Feb 2022 00:45:02 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c8719a7763019cd6d91cecde1c38293354d08a5257bc9ef0ee89b8cedfd253`  
		Last Modified: Wed, 02 Feb 2022 00:45:30 GMT  
		Size: 366.2 MB (366206994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685459e4b9dfe6aaafd370b1b2bebf8a4b802b452ffb3c8852fbb95ea48dc5a5`  
		Last Modified: Wed, 02 Feb 2022 00:45:03 GMT  
		Size: 532.2 KB (532245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eb6a70249f9e9b881dd73e800cac0fb7945d8e0ee86791e317af47157a7ef6`  
		Last Modified: Wed, 02 Feb 2022 00:45:02 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:7feeaafaa4d61b8585310d254244ae92b267780892b65d85ace0b449c5593284
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3079666838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a32e5aa5b5b992a35a509d0bce2cfc520c8db18f64da379bf3ec3489b129ad4`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 01 Feb 2022 22:28:23 GMT
ENV JAVA_VERSION=jdk-11.0.14+9
# Tue, 01 Feb 2022 22:30:29 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.14_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.14_9.msi ;     Write-Host ('Verifying sha256 (067ff937c3220c5c5fc5c75d82061e99dd6f60d50561c565d231670a8b5e510b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '067ff937c3220c5c5fc5c75d82061e99dd6f60d50561c565d231670a8b5e510b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Tue, 01 Feb 2022 22:31:25 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Tue, 01 Feb 2022 22:31:26 GMT
CMD ["jshell"]
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
	-	`sha256:7f60d6b06808d77257c6c2f43a388f8dd88e40abbab1f18030d541e4583d0e7b`  
		Last Modified: Wed, 02 Feb 2022 00:45:42 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba8d096c3a38b558dc2458f04322782dd31752348326cec246ff41e7ae9a1e1`  
		Last Modified: Wed, 02 Feb 2022 00:46:11 GMT  
		Size: 366.0 MB (366004195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c539b818422f3ce809afcc314bb6258240e7b2fe548585518b38f51d1a8a604`  
		Last Modified: Wed, 02 Feb 2022 00:45:42 GMT  
		Size: 336.9 KB (336923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f9642217034d16f58013a506fbe3a1b8b53e1e490fa9b27991808dcf61c16`  
		Last Modified: Wed, 02 Feb 2022 00:45:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
