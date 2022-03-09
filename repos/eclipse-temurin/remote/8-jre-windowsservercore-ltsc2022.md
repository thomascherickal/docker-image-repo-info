## `eclipse-temurin:8-jre-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:80c775b10b657bde8cb0b1bffc3af0244b8d0695f2a9d3fdfe9130b0e3de584e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `eclipse-temurin:8-jre-windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull eclipse-temurin@sha256:83b55aa5071016470c2efa1854c3c265934551f1342cf1261bad9cbadf5df671
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2292653663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:578a667b6fe17c9735283d0691507159f453c580bf0e54d164f0bd58dd38d712`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Mar 2022 21:50:39 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Tue, 08 Mar 2022 21:57:49 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_windows_hotspot_8u322b06.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_windows_hotspot_8u322b06.msi ;     Write-Host ('Verifying sha256 (74eb66d2d6aefdc42f95681616c94f6a41b1e133d899131719cf8c2f0cbf0a25) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '74eb66d2d6aefdc42f95681616c94f6a41b1e133d899131719cf8c2f0cbf0a25') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Tue, 08 Mar 2022 21:58:12 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db10fb44446c38d141f723d8a3067ecb9355e776aa4f36582f2b6ed192f898ca`  
		Last Modified: Tue, 08 Mar 2022 22:32:49 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b83b0161147c13e83707f659f4a99721f43a0ec50960126b79d3d9d8c3d6f99`  
		Last Modified: Tue, 08 Mar 2022 22:37:55 GMT  
		Size: 70.9 MB (70878334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4b4701472d5809a76ba8cd861ded14525451e1ed3296ca2c1a62c0fa9efa21`  
		Last Modified: Tue, 08 Mar 2022 22:37:45 GMT  
		Size: 525.6 KB (525596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
