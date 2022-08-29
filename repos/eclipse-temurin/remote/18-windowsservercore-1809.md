## `eclipse-temurin:18-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:8f899d75e2cd925db4af91010dedd6a8d47e53286fec8c8d1565512264bda4a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `eclipse-temurin:18-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull eclipse-temurin@sha256:8652d163c95556193382a32a54eb74c2478ec940491c50919f24a6c00ec2de8a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (3036434679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7561dcc73696bc95e406f77ae950555965b9d402de080fc16583ba7a7d7d73d9`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 29 Aug 2022 18:20:26 GMT
ENV JAVA_VERSION=jdk-18.0.2.1+1
# Mon, 29 Aug 2022 18:22:19 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2.1%2B1/OpenJDK18U-jdk_x64_windows_hotspot_18.0.2.1_1.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2.1%2B1/OpenJDK18U-jdk_x64_windows_hotspot_18.0.2.1_1.msi ;     Write-Host ('Verifying sha256 (e766c2d6100e70786ff0bb154054dd64bb45ea14ffc995544bbced98eb1c8703) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e766c2d6100e70786ff0bb154054dd64bb45ea14ffc995544bbced98eb1c8703') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-18' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 29 Aug 2022 18:23:25 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Mon, 29 Aug 2022 18:23:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9e3cf01955bdab0b3a5d34166f0b2654f5cda23e03dd4b953604b74a10965a`  
		Last Modified: Mon, 29 Aug 2022 18:35:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e92b39be5e8e185583d372595b8366ff6626c86de66ba74bd0f8b17385d5d3`  
		Last Modified: Mon, 29 Aug 2022 18:35:30 GMT  
		Size: 354.9 MB (354916666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af0e379987e7b538fbc1f796217c59c898badf45f391fe4482cf8b3f8d28f11`  
		Last Modified: Mon, 29 Aug 2022 18:35:04 GMT  
		Size: 3.8 MB (3800999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed65b4d503d1443119215799b6f794f728748ceb8bc63030b681f3211c5322f4`  
		Last Modified: Mon, 29 Aug 2022 18:35:03 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
