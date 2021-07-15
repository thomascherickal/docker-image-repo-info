## `adoptopenjdk:16-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:9c822e2437abd9cdf1d0ddb3fb7bc495b8bd63cd50ff20220c189ccc673176dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `adoptopenjdk:16-openj9-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull adoptopenjdk@sha256:3fa19b7f17b53742aea22dd4e24d2ee4443505b626ec1f83f81c454c8e75af67
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3075724026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed493b9b4207d98bf325d5e9beee28e7b19c854f180978d06d68fd93f971a146`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 16:25:35 GMT
ENV JAVA_VERSION=jdk-16.0.1+9_openj9-0.26.0
# Wed, 14 Jul 2021 16:27:33 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jdk_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jdk_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi ;     Write-Host ('Verifying sha256 (3aac3769355c1a427947705ef56ff8fcb5d412fdc3afc82c0778a92e643d6303) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '3aac3769355c1a427947705ef56ff8fcb5d412fdc3afc82c0778a92e643d6303') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jul 2021 16:27:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 14 Jul 2021 16:27:40 GMT
CMD ["jshell"]
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
	-	`sha256:0631565fbd0fcfe16289211cb49dd26166e8301b52595465bf804634a2702efc`  
		Last Modified: Wed, 14 Jul 2021 17:28:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74db1d8982371eb26b8e80886b27f1e3b3c7776b3314c46c150a5455d1ddb476`  
		Last Modified: Wed, 14 Jul 2021 17:36:00 GMT  
		Size: 390.3 MB (390271528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16707398989afd0c7a90c02ffcc86920df34d92ce0cb1c42ccf006569052fc5`  
		Last Modified: Wed, 14 Jul 2021 17:28:42 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1a96181599d3038a768e722f030e434384424c4e1a4cfe38ebcb5b3ac07784`  
		Last Modified: Wed, 14 Jul 2021 17:28:42 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
