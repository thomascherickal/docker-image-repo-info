## `eclipse-temurin:18-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:5511dc015eacec0680d2883913b259f8ee7ae0e51031cdecd7d2280e849c27e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `eclipse-temurin:18-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull eclipse-temurin@sha256:f5160c501acb170550c8e994faab2f76b8e9da310203fda57524931282a1f142
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2862573231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50d17667fb21cdd7ed89b99f93fc3bcdb178a4fb2b5bdfaaddc750bd9a41869b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 15:13:55 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 11 May 2022 15:15:13 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_windows_hotspot_18.0.1_10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_windows_hotspot_18.0.1_10.msi ;     Write-Host ('Verifying sha256 (6915a747550facec2cbfb22f6ae8f3c47dfcde857e69cf94409b664f81415e69) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '6915a747550facec2cbfb22f6ae8f3c47dfcde857e69cf94409b664f81415e69') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-18' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 May 2022 15:16:53 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 11 May 2022 15:16:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df51ff7ba754dd03b48706b43f7937a7122050287baef6e1cb1e58c077b43d64`  
		Last Modified: Wed, 18 May 2022 13:33:35 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eeedfbf47711e72051eb991dba4402b0c0200eb5b53978ee31077ed55d2bb9`  
		Last Modified: Wed, 18 May 2022 13:40:27 GMT  
		Size: 354.7 MB (354721582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16b1869edefb47838750d262f3f167981fb466bbdf7767cebdced25005cc49a`  
		Last Modified: Wed, 18 May 2022 13:33:39 GMT  
		Size: 3.8 MB (3791542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ab7d8b4b8d1b4e00fb347d093d71239d0177242c9e08401ee8b135e935e6d8`  
		Last Modified: Wed, 18 May 2022 13:33:35 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
