## `eclipse-temurin:17-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:7c3d2bcd702046c66e4040217a8b17a99c955a2a145ae3841bd724692944e273
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `eclipse-temurin:17-jdk-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull eclipse-temurin@sha256:132506dbf04ee9085cb1c2a0015dddcd9aafc73affc9652ffb56c2386f4279a4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3062195856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fec8f1b16a7c3816ce0cfba95dd87903d5cb9e09a5b2ce8aa05921b7f91c16e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 17:45:47 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 10 Nov 2021 17:47:23 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_x64_windows_hotspot_17.0.1_12.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_x64_windows_hotspot_17.0.1_12.msi ;     Write-Host ('Verifying sha256 (f5241bb43b589e45b6c3133fae6cc8cbffec4cae2504c3b99c3fac0c50cbf11e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f5241bb43b589e45b6c3133fae6cc8cbffec4cae2504c3b99c3fac0c50cbf11e') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Nov 2021 17:48:22 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 10 Nov 2021 17:48:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01134b41f534413e5cf9cf3d5ee946f4e033186e1d96126d6354280932f44552`  
		Last Modified: Wed, 10 Nov 2021 18:52:05 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8227ff6daf277e95bd04ca672dadca0383c2bc27f3557fe76a1aacb891b6e7d7`  
		Last Modified: Wed, 10 Nov 2021 18:52:34 GMT  
		Size: 352.2 MB (352181741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74548e18ef7cc5d25f8f4348bf2a4e7ab0ff710dcce670eee52b2bd05d507830`  
		Last Modified: Wed, 10 Nov 2021 18:52:07 GMT  
		Size: 3.9 MB (3888719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892cb41258316e8fdc50f54deb46015c04e9e03410c9fc85b92bc9b9d8912e31`  
		Last Modified: Wed, 10 Nov 2021 18:52:05 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
