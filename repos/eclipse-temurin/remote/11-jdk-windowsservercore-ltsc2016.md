## `eclipse-temurin:11-jdk-windowsservercore-ltsc2016`

```console
$ docker pull eclipse-temurin@sha256:c145a0039a78eaf01a843f45679be0f968d956224717a52f7b2f8ba100fd59ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `eclipse-temurin:11-jdk-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull eclipse-temurin@sha256:e0f6eff97c52b98daf8bf995ad180dfc5ada79e6b8885f08b1c1b1b02b83407f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6639071614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad2912f7d139b03174482a55bbc5abd54d0c0f1b09d754728ec18203fa4176f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 17:27:58 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 10 Nov 2021 17:29:42 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_windows_hotspot_11.0.13_8.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.13%2B8/OpenJDK11U-jdk_x64_windows_hotspot_11.0.13_8.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (b0edea638fd58c94d80abffd10bbb27731bf6fe1e2b3a9214fb68ab18237deed) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b0edea638fd58c94d80abffd10bbb27731bf6fe1e2b3a9214fb68ab18237deed') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Nov 2021 17:30:45 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 10 Nov 2021 17:30:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2def459ed8411492712c22025ea31e045244ac7b4940c522c445928b303c3752`  
		Last Modified: Wed, 10 Nov 2021 18:20:35 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e3cc1ac520d7d65a6069837a1f97f14fa0fdbe32cc94fdc0aff285c8ec3353`  
		Last Modified: Wed, 10 Nov 2021 18:27:16 GMT  
		Size: 365.7 MB (365654330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fccd435e6b40ce8019f505f543906f90455478cd9f2ee16821dd17644e38134`  
		Last Modified: Wed, 10 Nov 2021 18:20:35 GMT  
		Size: 322.2 KB (322190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24292f06bb6349a407bc14c6461791cc1cd08c218a68c26ffe0efc63df454c16`  
		Last Modified: Wed, 10 Nov 2021 18:20:35 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
