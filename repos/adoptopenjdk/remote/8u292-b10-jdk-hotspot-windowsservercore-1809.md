## `adoptopenjdk:8u292-b10-jdk-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:0e1002cf5d16b9009689ba9681588b31e79d6f2c0d68400e0856bdb38e1c0f9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `adoptopenjdk:8u292-b10-jdk-hotspot-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull adoptopenjdk@sha256:3f794561bf85f8af3264a6f2e9eabcbfd2b1b13090fc5717df9150cca53aacb6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2672426911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4065cde95191a877df96068b8e21c2d51104f4d567e202ccc3a040aada1b4111`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 17:37:20 GMT
ENV JAVA_VERSION=jdk8u292-b10
# Wed, 12 May 2021 17:38:42 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_windows_hotspot_8u292b10.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10/OpenJDK8U-jdk_x64_windows_hotspot_8u292b10.msi ;     Write-Host ('Verifying sha256 (f6bd2e351a451b8dc7ed19d44b18a27ff8a0602016625fac5134c4defe5e560c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f6bd2e351a451b8dc7ed19d44b18a27ff8a0602016625fac5134c4defe5e560c') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4850affec9717aa76f17b1708a82a204074fe1e1288ddb43fb790c40690b7552`  
		Last Modified: Wed, 12 May 2021 18:45:59 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49d124b9acb0b27e320bac39c3b56684227fbc75c8f1b38a5cb057c975a5afc`  
		Last Modified: Wed, 12 May 2021 18:54:53 GMT  
		Size: 197.9 MB (197934931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
