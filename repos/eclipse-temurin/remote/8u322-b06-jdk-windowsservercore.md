## `eclipse-temurin:8u322-b06-jdk-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:418aefc84ca1544b356a5e9fe07c79056d0c682583e9a56bca69ca70bbfff5d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `eclipse-temurin:8u322-b06-jdk-windowsservercore` - windows version 10.0.20348.587; amd64

```console
$ docker pull eclipse-temurin@sha256:d2339688f2030ff147c615d1688666532cb7a6cd59dda6fa1b4d51ebf7429a9f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2411383313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:620ae539b72384af90f59f72be32360444b8b65e2250debe14b0e40f553b111e`
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
# Tue, 08 Mar 2022 21:52:20 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_windows_hotspot_8u322b06.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_windows_hotspot_8u322b06.msi ;     Write-Host ('Verifying sha256 (e9337d5bba9b60a9d00a939fecb05718b2303023a587da6ae4862080714f9f0b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e9337d5bba9b60a9d00a939fecb05718b2303023a587da6ae4862080714f9f0b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Tue, 08 Mar 2022 21:53:08 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:faaf47d6529f3f700785980a827df3f9e17b9f755bc15d05ff2f3fce61e1c6dc`  
		Last Modified: Tue, 08 Mar 2022 22:36:32 GMT  
		Size: 189.6 MB (189608184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3291f628130f641198ac416083eb88185255f18d43aa0566b717aae5538083f8`  
		Last Modified: Tue, 08 Mar 2022 22:32:49 GMT  
		Size: 525.4 KB (525396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u322-b06-jdk-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull eclipse-temurin@sha256:d795e9fae83d61c1b72450f999a5e0d3a40f5b1af68b73fafc99a36dfcfa2a6d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2905160129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77d8ee85f3f1356633ef1f2b215af71083b98d83cbf86af5b33daf09733b16b3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Mar 2022 21:53:21 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Tue, 08 Mar 2022 21:54:47 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_windows_hotspot_8u322b06.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_windows_hotspot_8u322b06.msi ;     Write-Host ('Verifying sha256 (e9337d5bba9b60a9d00a939fecb05718b2303023a587da6ae4862080714f9f0b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e9337d5bba9b60a9d00a939fecb05718b2303023a587da6ae4862080714f9f0b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Tue, 08 Mar 2022 21:56:01 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24088d216953a30bdd9d5a1156e3c4da6792970f13293caf3acab5f4f2c65dc8`  
		Last Modified: Tue, 08 Mar 2022 22:36:46 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f911b94bcdedbadff1ef44deec5c2c8559be0782614e7f3b0a1abb24d6fdbf`  
		Last Modified: Tue, 08 Mar 2022 22:37:04 GMT  
		Size: 189.4 MB (189387966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec23de7dc8488d44abe07ef00a9d58fb980162b95f5055e26a03d18326160e0a`  
		Last Modified: Tue, 08 Mar 2022 22:36:47 GMT  
		Size: 316.9 KB (316930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
