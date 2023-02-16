## `eclipse-temurin:17-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:0b7578ac22aaefa1bc2b0113710beab701046cfa2ae62007ac1346433765c872
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `eclipse-temurin:17-windowsservercore-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull eclipse-temurin@sha256:96829dc744bed4f1e86ff6ead4418d19dfe6aeb614231e7e9c2216de3ae6c83b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2319572326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871b660ce1764ed4d7740d112f9bb79c05ac0d08b2d1986db9658cdcaf19c771`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Feb 2023 23:09:50 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Wed, 15 Feb 2023 23:12:01 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_windows_hotspot_17.0.6_10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_windows_hotspot_17.0.6_10.msi ;     Write-Host ('Verifying sha256 (943152d548f8dd24e3c07e67ddc17262d15dc390197cb4ef330867fe4130e590) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '943152d548f8dd24e3c07e67ddc17262d15dc390197cb4ef330867fe4130e590') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 15 Feb 2023 23:13:38 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 15 Feb 2023 23:13:40 GMT
CMD ["jshell"]
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
	-	`sha256:7a79e91bd2d4ff7c3f444a4aff8abc6187f479994915234c98ff3121abbe22da`  
		Last Modified: Thu, 16 Feb 2023 07:15:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade21027f0064d317b6c8fc367cfc619cb9b1dd660e2e64c808665965b423406`  
		Last Modified: Thu, 16 Feb 2023 07:15:42 GMT  
		Size: 352.7 MB (352696358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75cbeac15c44ddc19be5e19d42b2445b6ba790b6a536b33f4e5a08bdf936968`  
		Last Modified: Thu, 16 Feb 2023 07:15:06 GMT  
		Size: 3.9 MB (3913807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d2b2d71236a24e2821a873f8919fbc8a9b2715f98d553e74cab4ad269b575b`  
		Last Modified: Thu, 16 Feb 2023 07:15:04 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
