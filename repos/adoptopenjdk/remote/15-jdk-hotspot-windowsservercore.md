## `adoptopenjdk:15-jdk-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:470bc6ee804913b30866c8d0c4c329acf36274d7e18c87c057d3695622f96aa4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `adoptopenjdk:15-jdk-hotspot-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull adoptopenjdk@sha256:2e84edd515fb2146ad57e97dd8e11e6adf2b293c3d555eecfe73abfd2047b6d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 GB (3054341280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:317c31ec6fdd27e0376614c1fc9ffd776bbecccca751d418f9ffdc3e5a941bc9`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:41:54 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Wed, 14 Jul 2021 15:43:49 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_windows_hotspot_15.0.2_7.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_windows_hotspot_15.0.2_7.msi ;     Write-Host ('Verifying sha256 (bff27f4c7b8b562e5ab11b43b1fd257be89fab5779a68fb5cbef1d42a95ff449) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'bff27f4c7b8b562e5ab11b43b1fd257be89fab5779a68fb5cbef1d42a95ff449') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jul 2021 15:43:52 GMT
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
	-	`sha256:5ce6df93f815a40de3f547d56761345861bc8bd00382ec86438652d1e237aa20`  
		Last Modified: Wed, 14 Jul 2021 16:53:10 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d029770b015cbccff7673fe92a65f6e0d5f1421b9fa788382799e984d8731130`  
		Last Modified: Wed, 14 Jul 2021 16:53:41 GMT  
		Size: 368.9 MB (368890205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88e2d08764337360a47067047360354e1be0e66ffdf1829b8c5e409009ab387`  
		Last Modified: Wed, 14 Jul 2021 16:53:11 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jdk-hotspot-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull adoptopenjdk@sha256:92c25d966220b5249443566bdba5c85851bde09a6da2679dcb9b59860b607b11
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6638461538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07404b405233d891d650f67766ae72a781895dde6082c9a72cfc16e9b11f6b7c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:44:07 GMT
ENV JAVA_VERSION=jdk-15.0.2+7
# Wed, 14 Jul 2021 15:46:25 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_windows_hotspot_15.0.2_7.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7/OpenJDK15U-jdk_x64_windows_hotspot_15.0.2_7.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (bff27f4c7b8b562e5ab11b43b1fd257be89fab5779a68fb5cbef1d42a95ff449) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'bff27f4c7b8b562e5ab11b43b1fd257be89fab5779a68fb5cbef1d42a95ff449') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jul 2021 15:46:28 GMT
CMD ["jshell"]
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
	-	`sha256:8251f66e6b3e3c9f703ddcda7d3490340fc0c9c6717d3e0aaaa9d1f15811f31a`  
		Last Modified: Wed, 14 Jul 2021 16:53:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd44b1107c3b760fe58f281387388b1fd8112bf44e6ef96d7599fe547202dec6`  
		Last Modified: Wed, 14 Jul 2021 17:00:41 GMT  
		Size: 368.8 MB (368825335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d7e4210f3c1a6557bfdcd3f433ecd7f035a08f98e3cd98f3feb852da10cf02`  
		Last Modified: Wed, 14 Jul 2021 16:53:53 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
