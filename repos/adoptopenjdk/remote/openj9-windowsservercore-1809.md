## `adoptopenjdk:openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:19e66976f18a1424284d3595ce20bd64bb072aff75fcf2864504ffd4e17017ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `adoptopenjdk:openj9-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull adoptopenjdk@sha256:d6bffe8eeffca361e8dcd998a5c7319174bac25c9f7a9eabdc800037814ec374
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2864757578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb19c42f4dddd7464a97735c75cd57d6f0e54371430f4df37ef5c876b84cdaa`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 10 May 2021 18:57:09 GMT
ENV JAVA_VERSION=jdk-16.0.1+9_openj9-0.26.0
# Mon, 10 May 2021 18:59:00 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jdk_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jdk_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi ;     Write-Host ('Verifying sha256 (3aac3769355c1a427947705ef56ff8fcb5d412fdc3afc82c0778a92e643d6303) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '3aac3769355c1a427947705ef56ff8fcb5d412fdc3afc82c0778a92e643d6303') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 10 May 2021 18:59:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 10 May 2021 18:59:04 GMT
CMD ["jshell"]
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
	-	`sha256:37bfd0de287daada62afa22dd5724b893c505656839c271c75be3e275e34ef6e`  
		Last Modified: Mon, 10 May 2021 19:40:13 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cac281f27b19e918915e222ef23fddff3fb3e70f4a06dbfafe8ccefac7c5bed`  
		Last Modified: Mon, 10 May 2021 19:40:50 GMT  
		Size: 395.0 MB (394998035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d302e80d292d70d7c4845c0762fb288f96f5e2a4ec374f1933e0bc81b8aec82`  
		Last Modified: Mon, 10 May 2021 19:40:13 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4690e0c9870443408edd8a028ed5034f22853cd96a5be09d96a57b0aa2e7d22`  
		Last Modified: Mon, 10 May 2021 19:40:13 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
