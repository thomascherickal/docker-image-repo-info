## `eclipse-temurin:11-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:0b7ef8895e619bb6341ef0b20175f50eaf9ca4862f13d91f89865df94a8b982e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:11-jdk-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:8f9c47a65e1c7b757971e24d9f529d114245891a5d91553d5704974d76dd26f0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2401046860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b61536ec5f26fbf4f75ca6cdf190cade9d0000ed38a9c932d774681e97ee08c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 30 Oct 2023 23:16:56 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 30 Oct 2023 23:18:39 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.21_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.21_9.msi ;     Write-Host ('Verifying sha256 (ccaa09811f488cf95340e2702e8d9176058a52e89808ae6e1a1d20de39e5ce34) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'ccaa09811f488cf95340e2702e8d9176058a52e89808ae6e1a1d20de39e5ce34') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 30 Oct 2023 23:19:37 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Mon, 30 Oct 2023 23:19:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f37d88dbb9b222e786fc66c093aa29f73fce7217afd329c52ad1553ba760c7`  
		Last Modified: Mon, 30 Oct 2023 23:48:19 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83c236aac1371c9616ee574d3051e96a64f2f2756f31b903278f7d2b79d928f`  
		Last Modified: Mon, 30 Oct 2023 23:48:42 GMT  
		Size: 369.2 MB (369154035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1ffed458c65f69b4e168fc6e6c6d9435ada28bddf6b0921bba3662264b04ef`  
		Last Modified: Mon, 30 Oct 2023 23:48:19 GMT  
		Size: 298.2 KB (298181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5ae8681129bed6c7068fdf08346ef67d339d544ddd44eff8bf7553dce5ff39`  
		Last Modified: Mon, 30 Oct 2023 23:48:19 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
