## `eclipse-temurin:20-jre-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:0d58bb728fba0cd916606fe1330bb77f6fd21e71f78d1f78de341b555186cdbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `eclipse-temurin:20-jre-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull eclipse-temurin@sha256:a1786d888782208592177f66e8129e69c8daec3448876cb2d606cb9ef49cbd0a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1853760253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57b4976ba3bfbc3da37e52fbc56e972e1b6a0a4780e6c526d4ab931a703a894a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:04:02 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 10 May 2023 01:10:24 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ;     Write-Host ('Verifying sha256 (2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-20' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 May 2023 01:10:44 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea79297797be3714ba8d07431560ddff07237b2f971b0b44db0c144814ec2b5`  
		Last Modified: Wed, 10 May 2023 07:01:27 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666dbbf3fba6df3e4f8f5764ad4ac01fcc99682b53c0c597558a234f584031ec`  
		Last Modified: Wed, 10 May 2023 07:03:23 GMT  
		Size: 78.5 MB (78499733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1e7fa912621b3df5a29b7a85a309475702062eba70e19695ecd0e2b7ba84c2`  
		Last Modified: Wed, 10 May 2023 07:03:13 GMT  
		Size: 276.2 KB (276211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jre-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull eclipse-temurin@sha256:6f3a2db656c8c258e5282108ccf164e348e4afbf4e33a514472c9c4824ebafc3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2153875539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9d6a7fa56593c8756fe42ea4365bf5f06ee0cd855ee6b434a9c4e5e329bff1c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:05:44 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 10 May 2023 01:12:20 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ;     Write-Host ('Verifying sha256 (2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-20' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 May 2023 01:13:22 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e5699d1183de5e5440c7b704d3473b2faa919914e77cf60c42e1bbef32993`  
		Last Modified: Wed, 10 May 2023 07:02:04 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cc672ad5d0eb671661f4ac01b0f7fa1d78a92b1ac8d5cb934895987bf41bca`  
		Last Modified: Wed, 10 May 2023 07:03:41 GMT  
		Size: 78.5 MB (78512856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dcb96f46633e34c452a3260ceda72c058e3b9042f99afdcfd8c40cb1d287973`  
		Last Modified: Wed, 10 May 2023 07:03:32 GMT  
		Size: 3.3 MB (3324628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
