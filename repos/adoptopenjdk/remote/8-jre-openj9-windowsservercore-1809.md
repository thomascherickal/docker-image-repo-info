## `adoptopenjdk:8-jre-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:0a21fe9e9909b5fea0d263f67c26e4c7bdcad60355d9d8f9b76d56047ede2870
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `adoptopenjdk:8-jre-openj9-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull adoptopenjdk@sha256:4ca4ff8f8b696cdaacf7632ee46a7dc967516ff564f0c1ff945c740b3db3f92c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2776727884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88143c995de425de5fe9ddd36dce8328a424beb3fba0f282983a43928a4254d9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:59:19 GMT
ENV JAVA_VERSION=jdk8u292-b10_openj9-0.26.0
# Wed, 14 Jul 2021 16:05:05 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jre_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jre_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ;     Write-Host ('Verifying sha256 (8decae9e065946cfc9a4b7f3c0ed61cfc6fe3076cdcbbbece33ef39c9ccef6e3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8decae9e065946cfc9a4b7f3c0ed61cfc6fe3076cdcbbbece33ef39c9ccef6e3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jul 2021 16:05:08 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ce6c6f1d83a8e25cef40d46c7cb2160348273672c607c6c3c29623d014324c`  
		Last Modified: Wed, 14 Jul 2021 17:05:35 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769b4a19e647c964369ab8ed6f00cb3dae6d9fea04efcca85df613cebc153b92`  
		Last Modified: Wed, 14 Jul 2021 17:10:39 GMT  
		Size: 91.3 MB (91276808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93186d053519da48c6cf5eb319e5c67bef05768f33b20f58d148a6716b8c2c5b`  
		Last Modified: Wed, 14 Jul 2021 17:10:28 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
