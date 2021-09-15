## `adoptopenjdk:16-jre-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:163530c4573ded8fe3b8ca9e2f943070d30c13bbb7ef97e5b13efb52a7d8a613
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `adoptopenjdk:16-jre-hotspot-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull adoptopenjdk@sha256:c8d287b4dc00d049f6baf532959f69f4bbe8876a7efed8b9a8378738b5baaeda
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2765327323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:434d5ee98b2e5fc8b9bfa5055127589ae56257be03dee2eb55ef8036f502be1e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 00:29:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 17:23:27 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Wed, 15 Sep 2021 17:28:06 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_windows_hotspot_16.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_windows_hotspot_16.0.1_9.msi ;     Write-Host ('Verifying sha256 (781effe3282321702e7a6e63a5aa7614060da26572f136525fff4ade2c1e9a21) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '781effe3282321702e7a6e63a5aa7614060da26572f136525fff4ade2c1e9a21') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92dd43eae724dbe7e9e517c7fded74c5920ae7eb160042055178ceadf1916505`  
		Last Modified: Wed, 15 Sep 2021 01:09:40 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338fdc53724098b3f8a0879683269a1ab4e1e279885e010649496940e46e5c82`  
		Last Modified: Wed, 15 Sep 2021 18:06:32 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2afbdb81f1a4cca3a5e3fc991de4dfededa4be63bf081c1a1b3b03a81ca8770`  
		Last Modified: Wed, 15 Sep 2021 18:08:12 GMT  
		Size: 78.6 MB (78626627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
