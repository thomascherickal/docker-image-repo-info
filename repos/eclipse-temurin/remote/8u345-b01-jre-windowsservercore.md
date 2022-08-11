## `eclipse-temurin:8u345-b01-jre-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:a91a535dfc76f2585cb36c297d92c41704c4338769844720c99edd2d523dc1d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `eclipse-temurin:8u345-b01-jre-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull eclipse-temurin@sha256:660920883fa306d4905d1dc20fa2efa3a7e9bb3025f8d985626b713d04de309a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2388708269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d5f17e045312e70e6bbc5bf19b67aef64b921605bd9c15c80dd911fe7df2c3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 11 Aug 2022 19:15:23 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 11 Aug 2022 19:21:53 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_windows_hotspot_8u345b01.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_windows_hotspot_8u345b01.msi ;     Write-Host ('Verifying sha256 (30253824132f22de22fef11242fc9cd7a183b5e09757bb57ad1d82c03d852a3c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '30253824132f22de22fef11242fc9cd7a183b5e09757bb57ad1d82c03d852a3c') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Thu, 11 Aug 2022 19:22:14 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e0e2dd6d67f1b8ed30ce1606e5716fed6ccb4320f91d2f508ce1a6c4275461`  
		Last Modified: Thu, 11 Aug 2022 19:31:11 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451af3e9bdccae0deb37ea0425578e063b782cb7bd9c1e8fe17a57ef4a2391f2`  
		Last Modified: Thu, 11 Aug 2022 19:32:43 GMT  
		Size: 71.2 MB (71245517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af68182836f2ca8d5e444982fbaa356133fb4f4e9715cb60302cc9ded5ef5e8`  
		Last Modified: Thu, 11 Aug 2022 19:32:35 GMT  
		Size: 570.8 KB (570759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u345-b01-jre-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull eclipse-temurin@sha256:5cf5c62aec3238b927e5a0ee394c159c1f429e99781029702b0d8af2617bccaa
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2749016090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ecbcb22a6f167f2f235fe768be0dcd1b27ecbb1b30f94c93f6e9e5fb96f434`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 11 Aug 2022 19:17:10 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 11 Aug 2022 19:23:43 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_windows_hotspot_8u345b01.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jre_x64_windows_hotspot_8u345b01.msi ;     Write-Host ('Verifying sha256 (30253824132f22de22fef11242fc9cd7a183b5e09757bb57ad1d82c03d852a3c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '30253824132f22de22fef11242fc9cd7a183b5e09757bb57ad1d82c03d852a3c') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Thu, 11 Aug 2022 19:24:40 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
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
	-	`sha256:01d875e078fae7eb20d0fb76130e2e165680c4a1f38e86ef8fe0b2ed27f02b7c`  
		Last Modified: Thu, 11 Aug 2022 19:31:40 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6a3bf5806dc56b111cb5e26b84387e1af59f1d1a3be314249205ff33e926af`  
		Last Modified: Thu, 11 Aug 2022 19:33:00 GMT  
		Size: 71.0 MB (70982852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e64fbe107281371b424a33dcdb710d89cf424479b19c43fa4667c58f6db525`  
		Last Modified: Thu, 11 Aug 2022 19:32:52 GMT  
		Size: 317.7 KB (317654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
