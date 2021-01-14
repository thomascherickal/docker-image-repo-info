## `adoptopenjdk:11-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:8a91bb03467b76466f00a267d6aae75e7cd00412df2a5bb4d1cc03106e0ce7b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `adoptopenjdk:11-hotspot-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull adoptopenjdk@sha256:2a2fe87e3fb8091e6328e830641baa637288c0260352a9057ac50cdb7e6e03ce
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2808217062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b6df14e49c4396e2879443f1df4a56d0672038c49ecc7d16240418844d294e8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 21:54:55 GMT
ENV JAVA_VERSION=jdk-11.0.9.1+1
# Wed, 13 Jan 2021 21:57:28 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jdk_x64_windows_hotspot_11.0.9.1_1.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9.1%2B1/OpenJDK11U-jdk_x64_windows_hotspot_11.0.9.1_1.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (e949c3a7d84e2423f2557e6be3f85058e1c9dc2b5615c8fb6189831e29ee2cd9) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'e949c3a7d84e2423f2557e6be3f85058e1c9dc2b5615c8fb6189831e29ee2cd9') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Jan 2021 21:57:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c5c898831c3fce164d66426bc34494f117af6bb9e73aeffcc543efbfde7ac8`  
		Last Modified: Wed, 13 Jan 2021 23:13:20 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7f4e395468aaf0bac313aa0a46ae535f1a05e13ae9d8bc94d7625e7832c7be`  
		Last Modified: Wed, 13 Jan 2021 23:13:51 GMT  
		Size: 372.4 MB (372441561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2816da3163ec1299f4a5a89e8597aa0ef40684843b355a094487861488bac5bd`  
		Last Modified: Wed, 13 Jan 2021 23:13:19 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
