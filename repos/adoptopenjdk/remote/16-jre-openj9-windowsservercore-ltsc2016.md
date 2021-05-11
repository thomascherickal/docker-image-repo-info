## `adoptopenjdk:16-jre-openj9-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:55a7607f2d6b4f38f49af12a098ca58b4e3e6f6cb2cc46e2f58635f7f7ac9677
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `adoptopenjdk:16-jre-openj9-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull adoptopenjdk@sha256:ccd73c8d941b811e16ec5ebddc67799ac8ce6b9e79b6f4ff17266bbc14c2ebda
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5874137119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0974d701b5bb80842e58fa6c9ae2e95692d1214aca75965604f651532eee3c8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 10 May 2021 18:59:23 GMT
ENV JAVA_VERSION=jdk-16.0.1+9_openj9-0.26.0
# Mon, 10 May 2021 19:05:55 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jre_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jre_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (053b565eca3d7fba931fd547e78da881bf142d09370bbeed80e4e3fa31c747a6) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '053b565eca3d7fba931fd547e78da881bf142d09370bbeed80e4e3fa31c747a6') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 10 May 2021 19:05:56 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3fc4f8417f814fde6888675674708773d02151bec64ff114631d59981dc1e5`  
		Last Modified: Mon, 10 May 2021 19:41:07 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ccb15126df144ff46e8e5b5aff8ef39a2b7c04d07dcbc53105e717428eb1c8`  
		Last Modified: Mon, 10 May 2021 19:42:48 GMT  
		Size: 79.2 MB (79248972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2dac86f41b9281a3e07d1ede14dadaf7e2badf83d7812889d87968e96d31067`  
		Last Modified: Mon, 10 May 2021 19:42:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
