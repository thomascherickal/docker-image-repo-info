## `adoptopenjdk:8u292-b10-jre-openj9-0.26.0-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:f02c582ad27b82b135e83bf78b5a0ae08fd562a479ceea9d784a682a749df8ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `adoptopenjdk:8u292-b10-jre-openj9-0.26.0-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull adoptopenjdk@sha256:fb449a7d91c822cf54f57f69a0dc61aec90abde2e01c9f210a3a2f44c28006c3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2565763834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce374fc8c45aeacb929cd2c74d231464d07d682e2e6e94a47037fcfcaac61d2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 10 May 2021 18:39:59 GMT
ENV JAVA_VERSION=jdk8u292-b10_openj9-0.26.0
# Mon, 10 May 2021 18:45:19 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jre_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jre_x64_windows_openj9_8u292b10_openj9-0.26.0.msi ;     Write-Host ('Verifying sha256 (8decae9e065946cfc9a4b7f3c0ed61cfc6fe3076cdcbbbece33ef39c9ccef6e3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8decae9e065946cfc9a4b7f3c0ed61cfc6fe3076cdcbbbece33ef39c9ccef6e3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 10 May 2021 18:45:21 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c2ef53c6a0a5de9e14afebacfd8b9e61d77951aea45bbfd7ed3065fa846dc0`  
		Last Modified: Mon, 10 May 2021 19:33:59 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a18e65f550e3aa42b9c1c3a3143502219981c9357b2b8fb0c41369e74be1b95`  
		Last Modified: Mon, 10 May 2021 19:35:39 GMT  
		Size: 96.0 MB (96005677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43d79722069a7982b7e81db497c1465d65b35949063cb705506ae9e4a94cd49`  
		Last Modified: Mon, 10 May 2021 19:35:26 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
