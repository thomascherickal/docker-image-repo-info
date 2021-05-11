## `adoptopenjdk:11-jre-openj9-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:2418062706532076e6c7bd1149669b07a005db96f49b31921ce8b006d47396a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `adoptopenjdk:11-jre-openj9-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull adoptopenjdk@sha256:d297b1e641707e995a6127e65b3c0071820070bdba49b06ce9f060266f300519
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2549116719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e63a6ca906348d1196222444567a7ce6772af2984225e16aa02432643a98062`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 10 May 2021 18:47:50 GMT
ENV JAVA_VERSION=jdk-11.0.11+9_openj9-0.26.0
# Mon, 10 May 2021 18:54:13 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_x64_windows_openj9_11.0.11_9_openj9-0.26.0.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_x64_windows_openj9_11.0.11_9_openj9-0.26.0.msi ;     Write-Host ('Verifying sha256 (dda931759a562f6f3259931778dca142633f69297bf4128a7858aef87d373bdf) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'dda931759a562f6f3259931778dca142633f69297bf4128a7858aef87d373bdf') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 10 May 2021 18:54:15 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd599dfc03584f7f8bd092e0e4f5f03212b4ab10a8902db18d2fd62497c8b8c`  
		Last Modified: Mon, 10 May 2021 19:36:14 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abed525f552437e71854258cc1e1f85686af7cf9e424b88574f5b446c83bb83`  
		Last Modified: Mon, 10 May 2021 19:38:14 GMT  
		Size: 79.4 MB (79358553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2552e033fe397161b1091ffae7aa78b379da9039e6a540db7344e5963a7c5a`  
		Last Modified: Mon, 10 May 2021 19:38:01 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jre-openj9-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull adoptopenjdk@sha256:7cdecdb51b9d777381141cc60f42a76c02576f04394ea93a57e2c42761ce20bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5874749936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aee823d73892e621f3d66d51a18aeab89f69eb528fc614d8ae6e9077f77098a0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 10 May 2021 18:50:03 GMT
ENV JAVA_VERSION=jdk-11.0.11+9_openj9-0.26.0
# Mon, 10 May 2021 18:56:27 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_x64_windows_openj9_11.0.11_9_openj9-0.26.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_x64_windows_openj9_11.0.11_9_openj9-0.26.0.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (dda931759a562f6f3259931778dca142633f69297bf4128a7858aef87d373bdf) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'dda931759a562f6f3259931778dca142633f69297bf4128a7858aef87d373bdf') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 10 May 2021 18:56:29 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f867a31eea35e548caf6bfb50fd27e6783b6895149566726a960860de1ed2d1`  
		Last Modified: Mon, 10 May 2021 19:37:05 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdf4c602bc982aab1fb79f0f6af0049cea550d8b4de1a3a701d4ba069444897`  
		Last Modified: Mon, 10 May 2021 19:39:56 GMT  
		Size: 79.9 MB (79861800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddda20e63ba57cf7b3196bf97c8816842bee8e5c752d02f5908f5d659bde207e`  
		Last Modified: Mon, 10 May 2021 19:38:25 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
