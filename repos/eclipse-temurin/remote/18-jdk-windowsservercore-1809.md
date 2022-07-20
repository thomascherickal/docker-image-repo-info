## `eclipse-temurin:18-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:2d521e162c4b01963261cf2501c4834fcc5b2a20aaa0a0b89a73a89f59e18b1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `eclipse-temurin:18-jdk-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull eclipse-temurin@sha256:6325f319d567c6679836faffc82858e40223c65716343e74ac92427119aa2e4e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (3030423619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b845c6efa41cf6becce449467674853ae4109e2053a0e444ea861c3b98c8ab`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jul 2022 15:14:49 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 13 Jul 2022 15:16:20 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_windows_hotspot_18.0.1_10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_windows_hotspot_18.0.1_10.msi ;     Write-Host ('Verifying sha256 (6915a747550facec2cbfb22f6ae8f3c47dfcde857e69cf94409b664f81415e69) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '6915a747550facec2cbfb22f6ae8f3c47dfcde857e69cf94409b664f81415e69') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-18' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Jul 2022 15:17:17 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 13 Jul 2022 15:17:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2aa14b1c77d2ca9e682bc6e13260d39a0a84bca547d53f5a7895f6fd72b5a6`  
		Last Modified: Wed, 20 Jul 2022 12:51:45 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54921b3b458b47990f851a6ae1f781e4d579f57c590f83543f4ca835bb68b25e`  
		Last Modified: Wed, 20 Jul 2022 12:52:18 GMT  
		Size: 354.6 MB (354589754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd0c3724a7e926d551d7368c04e891161d00a75107e4df6cb30b5504ebd3a55`  
		Last Modified: Wed, 20 Jul 2022 12:51:46 GMT  
		Size: 3.8 MB (3785838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e043d4a087650a03cf828e88b3b239c152ce8fda298e95491182bf8cd571ce3c`  
		Last Modified: Wed, 20 Jul 2022 12:51:45 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
