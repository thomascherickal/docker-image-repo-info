## `eclipse-temurin:17-windowsservercore-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:15da8c7ae9f443a316c01b7f8170c95eb139624f66838d1ae31020e1a0abeaa5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.350; amd64

### `eclipse-temurin:17-windowsservercore-ltsc2022` - windows version 10.0.20348.350; amd64

```console
$ docker pull eclipse-temurin@sha256:21375adea736e2c71fa7217efe4022754b4485676703997e6b39888a4ec441c6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2537577934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26bf782cb632ba27e745339dbeef08e4cd8cc9c2fd16e7853bde2a7be87fdb82`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Wed, 03 Nov 2021 08:36:33 GMT
RUN Install update ltsc2022-amd64
# Wed, 10 Nov 2021 01:38:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 17:44:05 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 10 Nov 2021 17:45:11 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_x64_windows_hotspot_17.0.1_12.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_x64_windows_hotspot_17.0.1_12.msi ;     Write-Host ('Verifying sha256 (f5241bb43b589e45b6c3133fae6cc8cbffec4cae2504c3b99c3fac0c50cbf11e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f5241bb43b589e45b6c3133fae6cc8cbffec4cae2504c3b99c3fac0c50cbf11e') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-17' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Nov 2021 17:45:33 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac --version'; javac --version;     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
# Wed, 10 Nov 2021 17:45:33 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0eb404f1860fa8786ad09d1d9fe9fd580115f83cd38623bc4eb0c46abdaa0a3`  
		Size: 932.9 MB (932907933 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:27ded59d7006d9d7bffa7c253cd04a900a5d6b0d47b84d0edd624d12fd64cdc9`  
		Last Modified: Wed, 10 Nov 2021 02:07:39 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbcec8bf8a1afbf581516811c83e090535b44bcee64b0da8858fedddf3c1d4c`  
		Last Modified: Wed, 10 Nov 2021 18:45:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b52293b998db53bf4dc1e80d060a5f6a972dc763e936b6de619cbedbbf891d`  
		Last Modified: Wed, 10 Nov 2021 18:51:52 GMT  
		Size: 352.4 MB (352403355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e031cc7b63e95095b03559701e1e4820d6795e7ac1fd51812e57ccbac420e956`  
		Last Modified: Wed, 10 Nov 2021 18:45:25 GMT  
		Size: 563.3 KB (563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800aff4cb4ec07b18229df7c8be958615f8602af93a1af59d5547be7baa04468`  
		Last Modified: Wed, 10 Nov 2021 18:45:24 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
