## `adoptopenjdk:openj9-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:ca7c6c08b49041e5e76c4dc5925b067aa3253effddd43927d8cdf467d9b7d418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `adoptopenjdk:openj9-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull adoptopenjdk@sha256:698d9ac97cb547853d54a30de005056c1537be7e99e4e9cf1f24f64f1efca5f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 GB (6661156585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba3fc1922e4e390df104f3b1825dd00d35242e40c549be2a462326be5cc6afc8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 19:49:38 GMT
ENV JAVA_VERSION=jdk-16.0.1+9_openj9-0.26.0
# Wed, 11 Aug 2021 19:51:57 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jdk_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jdk_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (3aac3769355c1a427947705ef56ff8fcb5d412fdc3afc82c0778a92e643d6303) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '3aac3769355c1a427947705ef56ff8fcb5d412fdc3afc82c0778a92e643d6303') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 Aug 2021 19:52:00 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 11 Aug 2021 19:52:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84aba1cf981fd8edbd49b9bd6d53250fdf5fc7cdfa1ed4baadd9fe52ec6662f3`  
		Last Modified: Wed, 11 Aug 2021 20:54:48 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb9c250452d4383d7612fe4e171bb803ba8bdf559a0708e8f1cd3a45a7d728d`  
		Last Modified: Wed, 11 Aug 2021 20:55:18 GMT  
		Size: 390.2 MB (390184931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6db296b3e46b7a8e65dcdad306efa26bb8ef6f16aa6cfd953857086d9dcea0`  
		Last Modified: Wed, 11 Aug 2021 20:54:50 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9deba60d5c31fac7a27e50c86e61963b2e4b0fa9ea1849f8f9bb5c459b48b48`  
		Last Modified: Wed, 11 Aug 2021 20:54:48 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
