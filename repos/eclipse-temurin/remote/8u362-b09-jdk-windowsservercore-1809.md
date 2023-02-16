## `eclipse-temurin:8u362-b09-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:11c1ed8294169a7c5b4ea1a86635c444908df88e537c4d2a7d6849fcd4dbb9ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `eclipse-temurin:8u362-b09-jdk-windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull eclipse-temurin@sha256:ac524083054abad1d6d63b1001dd6524d469fc10d3972efaef1b66bd21a67341
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2154485493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f89d6c83ff65de6bc035c10ef9c0b72fb2e69aafc6905d09c394ea3b1370daea`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 22:41:29 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Wed, 15 Feb 2023 22:44:13 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_windows_hotspot_8u362b09.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_windows_hotspot_8u362b09.msi ;     Write-Host ('Verifying sha256 (07d6ff7bb5400a618e7e8c6e6104c04c1df6141fa85026526676aa8af011e44c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '07d6ff7bb5400a618e7e8c6e6104c04c1df6141fa85026526676aa8af011e44c') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 15 Feb 2023 22:46:03 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59e9e8f2bb7d2c294e2f59794a1a793a7d692467c690fbab1a2e31586d01c8e`  
		Last Modified: Thu, 16 Feb 2023 07:09:02 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05d891b7eada328052abd45db9d7bd14fd95d287cfdf8b816fe2c360b182328`  
		Last Modified: Thu, 16 Feb 2023 07:09:26 GMT  
		Size: 191.2 MB (191183826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61797b09eb5c032ec52cf17be373e7abb740565415dab3881998e8aac7a8d31e`  
		Last Modified: Thu, 16 Feb 2023 07:09:03 GMT  
		Size: 341.0 KB (341046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
