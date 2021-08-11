## `adoptopenjdk:hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:ea5e3b115ad34a19daf48d3cdb388709fe676021697e9ac16b2e34d49607dd2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `adoptopenjdk:hotspot-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull adoptopenjdk@sha256:fe935262199cff01f6461cf1de9f944c270099bb29abfc0a8b6c87a2c70d36d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3063966863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7750765deade9d5af600fcce259ff3bde1dcb7d0d80f9b3ea0cf4bd631502ac`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 19:12:17 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Wed, 11 Aug 2021 19:14:11 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_windows_hotspot_16.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jdk_x64_windows_hotspot_16.0.1_9.msi ;     Write-Host ('Verifying sha256 (dc898ec3574e08a90f67fa75808954462749c874ab22c860ded6de051bcc7499) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'dc898ec3574e08a90f67fa75808954462749c874ab22c860ded6de051bcc7499') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 11 Aug 2021 19:14:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e24c8c89f41bd2695a9dc52b1094085a6b5692b2ee1702370c80c986a20d380`  
		Last Modified: Wed, 11 Aug 2021 20:26:57 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c98b9b4cbf111fd931d0e918f1ccc673095272314e985406717b3b62281d7c9`  
		Last Modified: Wed, 11 Aug 2021 20:27:25 GMT  
		Size: 378.0 MB (377964646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19be57862606a7e0b77ad87e5c49021acf2fa63924a529c2c0def9183c9a404`  
		Last Modified: Wed, 11 Aug 2021 20:26:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
