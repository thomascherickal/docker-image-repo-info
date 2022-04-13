## `eclipse-temurin:11-jre-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:1fd700c43dfc6f55e51548b1be2bc7553a11434c2ed7c4bc190210d8e6d40b1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:11-jre-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:c26c156cef9d412069b0dd14dfb3393f6d4b577bc0b2a4857b5dcfb03aca6330
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2789911810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd996578a152ff1f5ee87c9e5f881279ba85fa9ee014da428222a66cf75c7c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 15:22:05 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Wed, 13 Apr 2022 15:27:41 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_windows_hotspot_11.0.14.1_1.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jre_x64_windows_hotspot_11.0.14.1_1.msi ;     Write-Host ('Verifying sha256 (8559c143021508f70885adc84b5be4ce56e4fe7d9d2b74ac45fc2effc841b92d) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8559c143021508f70885adc84b5be4ce56e4fe7d9d2b74ac45fc2effc841b92d') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-11' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Apr 2022 15:28:31 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a563fc975100842b60b99a9ab97cde427d3f1e7d879014b155ca995e0b72daff`  
		Last Modified: Wed, 13 Apr 2022 16:09:07 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e557266311d4bc28107a7d77c7d0cde797ad290eba16fc66197f5c63ab19f2`  
		Last Modified: Wed, 13 Apr 2022 16:20:11 GMT  
		Size: 73.7 MB (73656932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df67a865f475050c59b62a26a338e5459d98fbc5006beb11658072db6f15ddb1`  
		Last Modified: Wed, 13 Apr 2022 16:20:01 GMT  
		Size: 331.7 KB (331706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
