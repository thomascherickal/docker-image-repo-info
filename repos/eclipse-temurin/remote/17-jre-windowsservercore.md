## `eclipse-temurin:17-jre-windowsservercore`

```console
$ docker pull eclipse-temurin@sha256:ef7a51e36303a7ac6b541d2f8a53981aa30233fad33c1e027dc924b8d2aa25d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.469; amd64
	-	windows version 10.0.17763.2452; amd64

### `eclipse-temurin:17-jre-windowsservercore` - windows version 10.0.20348.469; amd64

```console
$ docker pull eclipse-temurin@sha256:65dd6e166d72f0e083c8c85c0df99e812be57ddbb80e1d77c95cc5ccca1aba4a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2282655885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee6ea4b20fd2c4e3fea55a863ccc137d4db6c46effd4e60bc10c1f4279bff47f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 06 Jan 2022 03:56:33 GMT
RUN Install update ltsc2022-amd64
# Tue, 11 Jan 2022 18:59:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 22:10:12 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Tue, 11 Jan 2022 22:22:04 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_x64_windows_hotspot_17.0.1_12.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_x64_windows_hotspot_17.0.1_12.msi ;     Write-Host ('Verifying sha256 (f1580b6aa2071448798d5f5e3c229fc150cb5bc4e650c365121be9afdf4c313b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f1580b6aa2071448798d5f5e3c229fc150cb5bc4e650c365121be9afdf4c313b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Tue, 11 Jan 2022 22:22:26 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b593686e27e7562a5b0696823307ffa822214cee8bd2eec1075eadad4cb9712`  
		Size: 956.0 MB (956001983 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:99e0b71ede60d3b2c5b9053bf27e47c0875590991eede49813d849cc660c7551`  
		Last Modified: Tue, 11 Jan 2022 19:32:06 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1498d4d35a3500452bedcca7cc551a1213859501a35f38cf58ea943a02a703dd`  
		Last Modified: Tue, 11 Jan 2022 23:03:51 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66335658d83376f9275d84556a60bbec7a9587f021edcde59c096f858a9864e7`  
		Last Modified: Tue, 11 Jan 2022 23:13:53 GMT  
		Size: 74.4 MB (74386145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ff2e4e2b3cb472f93239fd9e8a7bbead5257fa4a6dd7df2faff648ceaaba00`  
		Last Modified: Tue, 11 Jan 2022 23:12:35 GMT  
		Size: 566.0 KB (565966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-windowsservercore` - windows version 10.0.17763.2452; amd64

```console
$ docker pull eclipse-temurin@sha256:aacbe117ac067cabc3bd47acf6306998927ce43bc6b5f1c263064e16258f213e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2789596301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef3c21224a23b9c4a90cf4bd64a75490e7885073fad9a884f42f24934a99514a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 05:11:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 15:50:57 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 12 Jan 2022 15:57:08 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_x64_windows_hotspot_17.0.1_12.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_x64_windows_hotspot_17.0.1_12.msi ;     Write-Host ('Verifying sha256 (f1580b6aa2071448798d5f5e3c229fc150cb5bc4e650c365121be9afdf4c313b) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f1580b6aa2071448798d5f5e3c229fc150cb5bc4e650c365121be9afdf4c313b') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 12 Jan 2022 15:58:01 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3a70d5fd54e2005efbf590b48700ed40509210354a0d8f3f18c3b444a5325896`  
		Last Modified: Wed, 12 Jan 2022 06:20:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84188f71c0f864d1b3da7ba88819efc8d10d03f0c19352d71e040cf07c5a1786`  
		Last Modified: Wed, 12 Jan 2022 16:19:00 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfcf8ca954cf9189f2e47e09f282b4f8c7ffbcaa2fc7a68a27445bc05b443b0`  
		Last Modified: Wed, 12 Jan 2022 16:23:28 GMT  
		Size: 74.1 MB (74112266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7ea7ec17f2125d2ee673cb518b00f283646edb93e0e178c46e870a0f57747e`  
		Last Modified: Wed, 12 Jan 2022 16:23:19 GMT  
		Size: 3.3 MB (3250290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
