## `adoptopenjdk:11-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:3d677422a4b41e8d0a3370c86b443fbe0c328244c1cb193321cc48bbe1279a72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `adoptopenjdk:11-hotspot-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull adoptopenjdk@sha256:8c40ab8e2f3c15dddc03c5f715de838d2798d52cb25cd3378e8b38d120583389
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2838933195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97782b80cf0efd4980452eaf4d882a5281201fdb24bf125e88c2d5b6183d77c6`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 10 May 2021 18:23:01 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Mon, 10 May 2021 18:24:46 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.11_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.11_9.msi ;     Write-Host ('Verifying sha256 (de7de70fbd9f3ff49ce34db87c5f331a5c0b72e54c16e9e6d9ba3007d23b361e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'de7de70fbd9f3ff49ce34db87c5f331a5c0b72e54c16e9e6d9ba3007d23b361e') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Mon, 10 May 2021 18:24:47 GMT
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
	-	`sha256:54d2093d3e911cf6a5e76917eac57c67658476ee3f28936c082036167c43d451`  
		Last Modified: Mon, 10 May 2021 19:17:53 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba692c9e7369286cc34a3bb81f847ace2a6b0fc1c0e2bd09b32c837934b77324`  
		Last Modified: Mon, 10 May 2021 19:25:04 GMT  
		Size: 369.2 MB (369175059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb967d56cc5f1c2a2aaf98591c0b1d2faee490c7d98fd416221021bccdb2aca`  
		Last Modified: Mon, 10 May 2021 19:17:53 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
