## `eclipse-temurin:8-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:064d2bb790fc114dafb8f8d3e44e60790f323a63e084d5fc3a07d3e213b4f584
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `eclipse-temurin:8-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

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
