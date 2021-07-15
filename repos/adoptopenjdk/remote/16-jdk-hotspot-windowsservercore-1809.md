## `adoptopenjdk:16-jdk-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:760181f4a2092820d89e1af23266990588044f78101984e5297202b5e0440cfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `adoptopenjdk:16-jdk-hotspot-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull adoptopenjdk@sha256:50b55c594748ce304f5a0c5c310dce3f6a8a90102eaa653c5951417906dbc886
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3063428908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0dfdc3d41c67af9d3ddee8af8eef5fae372fb669c4a719cda077eab583edcb0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:50:59 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Wed, 14 Jul 2021 15:52:51 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_windows_hotspot_16.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_windows_hotspot_16.0.1_9.msi ;     Write-Host ('Verifying sha256 (dc898ec3574e08a90f67fa75808954462749c874ab22c860ded6de051bcc7499) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'dc898ec3574e08a90f67fa75808954462749c874ab22c860ded6de051bcc7499') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jul 2021 15:52:54 GMT
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
	-	`sha256:3c8233801d7b9d090726fc4f88542e680df88c6b4bcb6d7ea7dc3e1a08de8fb9`  
		Last Modified: Wed, 14 Jul 2021 17:03:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ace8ec8b7dc27b324ce63089986afa22fe9c297f8413c45dd2d6f4ebbde525`  
		Last Modified: Wed, 14 Jul 2021 17:03:50 GMT  
		Size: 378.0 MB (377977873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067b2cfbcddd3dcaa9271fa3f7569b96b81f32a2da181b9a4d4e005c96965b46`  
		Last Modified: Wed, 14 Jul 2021 17:03:21 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
