## `eclipse-temurin:11-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:eaf16717e97a228cc34eef6b5419b491958698097697dc10a2ab6cd220e05b5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `eclipse-temurin:11-jdk-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull eclipse-temurin@sha256:4fc365142d0e3295317f9388e5a606c21c76034be1b39519d1ed25f6ee100a51
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2870772242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2f72b2029317e94ad6ee2a6375013ce1201b708f4006c924f3d266c0e8b1f10`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 14:56:15 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Wed, 11 May 2022 14:57:42 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jdk_x64_windows_hotspot_11.0.15_10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.15%2B10/OpenJDK11U-jdk_x64_windows_hotspot_11.0.15_10.msi ;     Write-Host ('Verifying sha256 (083082efde2ebc3989549b350a6b2ada77713d58fb7e489f2ba23a34da387094) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '083082efde2ebc3989549b350a6b2ada77713d58fb7e489f2ba23a34da387094') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 May 2022 14:58:41 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 11 May 2022 14:58:42 GMT
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
	-	`sha256:daa97e011d2b042e2449f41a1c4c3a280ffeec9347739bd4988666acf4a9cbb5`  
		Last Modified: Wed, 18 May 2022 12:59:38 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bc0d7b3241a77e8769e8129eb559f4de4570c1069aeaf967e87447449ea7b0`  
		Last Modified: Wed, 18 May 2022 13:06:20 GMT  
		Size: 366.4 MB (366388137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6813ee22e3f90204f98e83954018bb4deab956056cfd269b77cc6b3a717228fd`  
		Last Modified: Wed, 18 May 2022 12:59:39 GMT  
		Size: 324.0 KB (323965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da303140c0266a7efcf24dde902b851d47b3448ba75a33c827b265f9a82f5e97`  
		Last Modified: Wed, 18 May 2022 12:59:38 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
