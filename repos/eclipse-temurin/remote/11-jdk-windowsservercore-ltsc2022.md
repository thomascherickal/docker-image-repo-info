## `eclipse-temurin:11-jdk-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:8bd727cd80565fc82978f2c416d8cd82b5b7dd2fa3c75fb8e3bdc4089f77e699
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:11-jdk-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:97612783497afe1b6bab1d7e3041d235fc51b3e7fbd165b5723ff39940a53aea
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1793631315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:771b8cdc8274d51d647f7057558ce9987e6935b3563ccd16b6a4c4dd6f574a1a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 00:45:32 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Sat, 24 Jun 2023 00:46:36 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_x64_windows_hotspot_11.0.19_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_x64_windows_hotspot_11.0.19_7.msi ;     Write-Host ('Verifying sha256 (8f8f136e2071591c6ea7bc58d629a5c8ad23c829bb1878200fdff0c0fe97712c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8f8f136e2071591c6ea7bc58d629a5c8ad23c829bb1878200fdff0c0fe97712c') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 24 Jun 2023 00:46:59 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Sat, 24 Jun 2023 00:47:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d4e28c1d2928452bdeb42928074a54917a77f5983ee5acd013a6969bd5d694`  
		Last Modified: Sat, 24 Jun 2023 01:26:05 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2981b4ed6410aeb78c81694d1597a4563b198c09605a47fcb43049ce266b535`  
		Last Modified: Sat, 24 Jun 2023 01:26:33 GMT  
		Size: 367.1 MB (367050962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157ff0d33e247405f3237b96b54a4670c0f89d6773822d71b80a2f0a1ac4b2f8`  
		Last Modified: Sat, 24 Jun 2023 01:26:05 GMT  
		Size: 277.7 KB (277721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ede6414014c7ebe2360a651bed02b37d7fc83058fb20c8d05c9c1ba6e61c7bb`  
		Last Modified: Sat, 24 Jun 2023 01:26:05 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
