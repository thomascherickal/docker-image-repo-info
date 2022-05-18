## `eclipse-temurin:11-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:6a40cca8aee48d0a934a145032e2c90ae8a92976380099636d46709fe6e6f296
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `eclipse-temurin:11-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull eclipse-temurin@sha256:a8e9f04e81f0cee3dc40298911f85eb169b10c9a6a75c049f889a059bb708624
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312018476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590b10af238984f34b3534c267063e8251b7c2a400304a5a9c05cb0cfe8df5cb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 14:54:33 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Wed, 11 May 2022 15:00:30 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_windows_hotspot_11.0.15_10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jre_x64_windows_hotspot_11.0.15_10.msi ;     Write-Host ('Verifying sha256 (8072ed7f0235920022bd49b104cc79652d0f01cdec608848a73a320c6192ad77) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8072ed7f0235920022bd49b104cc79652d0f01cdec608848a73a320c6192ad77') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 May 2022 15:00:54 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d164ba0837d67412d0f684782119bec8a4aea21188ecb119f99b972a5cc190`  
		Last Modified: Wed, 18 May 2022 12:52:44 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7591114f31d1798172716068014d17039946ad67e14d91e337407da3b466529a`  
		Last Modified: Wed, 18 May 2022 13:11:36 GMT  
		Size: 73.9 MB (73927537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7a70ad32a11e951fa43f3d31cb87ef7e65285ed4b1408eb45520a4e14cf565`  
		Last Modified: Wed, 18 May 2022 13:10:16 GMT  
		Size: 552.9 KB (552881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
