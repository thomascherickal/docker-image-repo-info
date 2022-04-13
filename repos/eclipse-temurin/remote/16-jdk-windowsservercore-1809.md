## `eclipse-temurin:16-jdk-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:3e37f462784a9d625b5d05d8f7c6dc06b13444b8697a610946e322e8fa4f2816
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:16-jdk-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:62e7fdbcb3c2a10e6cddadf678be7608c3d5ec815940ddb3484cfc662391218b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3098767337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:038a4c09b954394eaf55cd74d6db4fd7e875b342ae3cea43a85b04f94583f328`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 15:29:10 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Wed, 13 Apr 2022 15:30:51 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_windows_hotspot_16.0.2_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin16-binaries/releases/download/jdk-16.0.2%2B7/OpenJDK16U-jdk_x64_windows_hotspot_16.0.2_7.msi ;     Write-Host ('Verifying sha256 (b153c6ce102c6f05fd710c4b26c64224b649457613dad4830dcc6b551c0a4b3d) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b153c6ce102c6f05fd710c4b26c64224b649457613dad4830dcc6b551c0a4b3d') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-16' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Apr 2022 15:31:47 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 13 Apr 2022 15:31:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e53848a574fe266ee36b0e1a91a52c69fcf852ac88871a63c758e83c47d65a`  
		Last Modified: Wed, 13 Apr 2022 16:21:29 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905a1d6b52ea2b0a5647f596735dab7f14796e9afbb2c971cb877a9447571e0d`  
		Last Modified: Wed, 13 Apr 2022 16:21:57 GMT  
		Size: 378.9 MB (378911103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bece11f33d51516837b016266a55c0c7936601984c1291f60037be51202d5df7`  
		Last Modified: Wed, 13 Apr 2022 16:21:30 GMT  
		Size: 3.9 MB (3931765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f248cc3cd7a05e6e5e5720649deaa2348b25aba5ff527a628fdca6baea2a18c8`  
		Last Modified: Wed, 13 Apr 2022 16:21:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
