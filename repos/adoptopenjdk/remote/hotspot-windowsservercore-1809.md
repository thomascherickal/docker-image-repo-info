## `adoptopenjdk:hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:a732427d01ac8e65e66d680b1cc6eda73f0d8231794c1e0d82fd2276bf5799ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `adoptopenjdk:hotspot-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull adoptopenjdk@sha256:e6ef0f01aa01299212dbde99a603b5d1310d2c372bc5787bc08b679c95170612
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2852463987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8690db3b73513d22548c5d95dc7f2f32958ae3b8d325e8873cb32aa678d4535c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 10 May 2021 18:32:05 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Mon, 10 May 2021 18:33:44 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_windows_hotspot_16.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_windows_hotspot_16.0.1_9.msi ;     Write-Host ('Verifying sha256 (dc898ec3574e08a90f67fa75808954462749c874ab22c860ded6de051bcc7499) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'dc898ec3574e08a90f67fa75808954462749c874ab22c860ded6de051bcc7499') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 10 May 2021 18:33:46 GMT
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
	-	`sha256:085c21bdc6eacd3f6134aef396846db2731329096f702b7903f80c13b54d3db3`  
		Last Modified: Mon, 10 May 2021 19:28:24 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301ef67ac76bee7b4a0205d0669bbf15feec4aeaf7b6e8b38e90ce0d3f65ed3`  
		Last Modified: Mon, 10 May 2021 19:29:02 GMT  
		Size: 382.7 MB (382705825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9446863b0104714b6c1b46c5f8d627cfb78b67b933154c4dd88e3043bfe68027`  
		Last Modified: Mon, 10 May 2021 19:28:24 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
