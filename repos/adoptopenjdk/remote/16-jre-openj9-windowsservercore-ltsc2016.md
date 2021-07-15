## `adoptopenjdk:16-jre-openj9-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:2d39112ae0914c09dbd326b6f163fc0dae9455e3646a9936fa84ee770959ffbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `adoptopenjdk:16-jre-openj9-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull adoptopenjdk@sha256:a544ace8383cd0b3b58bde787508329665282a03ea74642b33cd566a740661f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6343579472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2094fc34f9d7bc42f86d15388bd011e15660ebcaecce72772f46d806a871fb2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 16:27:48 GMT
ENV JAVA_VERSION=jdk-16.0.1+9_openj9-0.26.0
# Wed, 14 Jul 2021 16:34:33 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jre_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9_openj9-0.26.0/OpenJDK16U-jre_x64_windows_openj9_16.0.1_9_openj9-0.26.0.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (053b565eca3d7fba931fd547e78da881bf142d09370bbeed80e4e3fa31c747a6) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '053b565eca3d7fba931fd547e78da881bf142d09370bbeed80e4e3fa31c747a6') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jul 2021 16:34:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819e49aed987abe67c0f6c1c20e31746a56bc001e6308314fe98dfaf0987ac04`  
		Last Modified: Wed, 14 Jul 2021 17:36:16 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dbfac8b056272d85396338f7787bd29764a6653060cfa65df6f4082f4a43b5`  
		Last Modified: Wed, 14 Jul 2021 17:45:53 GMT  
		Size: 73.9 MB (73943242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a10845b1ba58938815f73edf1358763df3d7aee881e9fd865f8b93b6c4df0f`  
		Last Modified: Wed, 14 Jul 2021 17:45:43 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
