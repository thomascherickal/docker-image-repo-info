## `adoptopenjdk:15-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:fe4ba33fe3067249acf3e11845707a0ecc2e69bc914ad1785d0ed687d316da8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `adoptopenjdk:15-hotspot-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

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
