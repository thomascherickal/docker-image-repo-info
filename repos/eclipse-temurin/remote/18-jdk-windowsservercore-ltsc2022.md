## `eclipse-temurin:18-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:cd69051cffcb2cc1939aed581d337da702395d3dab27ef947773af2bc5b38ea2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `eclipse-temurin:18-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:e4057722c7abe874920920fcb209bd804f64fba0e2833ef62ef0aca4f5236ad0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2582368128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:563d08d15066f08e0176391f4689b476fcc538cb36d2a76536227af8f3f0c293`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 04 May 2022 18:17:37 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 04 May 2022 18:18:53 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_windows_hotspot_18.0.1_10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_windows_hotspot_18.0.1_10.msi ;     Write-Host ('Verifying sha256 (6915a747550facec2cbfb22f6ae8f3c47dfcde857e69cf94409b664f81415e69) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '6915a747550facec2cbfb22f6ae8f3c47dfcde857e69cf94409b664f81415e69') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-18' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 04 May 2022 18:19:42 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 04 May 2022 18:19:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39da655b2390ca6c77bb41f8a18aba94d81f7ed3ca9716c950549ed4ddae8201`  
		Last Modified: Wed, 04 May 2022 18:32:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d2b54adb3a9f71bd9f48dd21194e82a3ba80ef31ad88602d0846e19939bba7`  
		Last Modified: Wed, 04 May 2022 18:32:34 GMT  
		Size: 354.8 MB (354832513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9cb1ec29b1b520f48adce391fc04ee06c96bb8d57d5b968d56aeab27ef31a5`  
		Last Modified: Wed, 04 May 2022 18:32:06 GMT  
		Size: 576.5 KB (576542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b1e2c5b36054ce277d5de0cb63d12c2f328af9ec015d5fcb6e763ee8f4ebb2`  
		Last Modified: Wed, 04 May 2022 18:32:06 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
