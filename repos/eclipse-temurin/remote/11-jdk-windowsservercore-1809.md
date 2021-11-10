## `eclipse-temurin:11-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:1cf12c0d67d7e82604ec56b0a17f92be5360408259e78c369de64924d1fc0185
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `eclipse-temurin:11-jdk-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull eclipse-temurin@sha256:f221e8b873471b631202a9b1192281e086d129aeaf06c2f239aafd5f0cbc07a2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3072173002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0f97c108aea475b6bf1d833a0b29a1017e55f25ba1bce6f8fb66ad1a21a704e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 17:24:32 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 10 Nov 2021 17:26:09 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_windows_hotspot_11.0.13_8.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_windows_hotspot_11.0.13_8.msi ;     Write-Host ('Verifying sha256 (b0edea638fd58c94d80abffd10bbb27731bf6fe1e2b3a9214fb68ab18237deed) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b0edea638fd58c94d80abffd10bbb27731bf6fe1e2b3a9214fb68ab18237deed') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Nov 2021 17:27:02 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 10 Nov 2021 17:27:03 GMT
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
	-	`sha256:7ec41d9bc2ecac35e54629bffb67532cedb5bd6fa8ac1b638d2e827366e8c836`  
		Last Modified: Wed, 10 Nov 2021 18:10:01 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e631dc05be92d13670a1e23bad4c5434e4ba2521c4489c66d26e5f63e635fe64`  
		Last Modified: Wed, 10 Nov 2021 18:16:37 GMT  
		Size: 365.7 MB (365719504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673d3d98e098e7fae5b612c0e59bddd0b965ecfea1f2320769c96d1804060431`  
		Last Modified: Wed, 10 Nov 2021 18:10:01 GMT  
		Size: 328.1 KB (328096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b390d0987887b1e2b226d3b0314e9be2875e36513685d677c09d026fdce61a3`  
		Last Modified: Wed, 10 Nov 2021 18:10:01 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
