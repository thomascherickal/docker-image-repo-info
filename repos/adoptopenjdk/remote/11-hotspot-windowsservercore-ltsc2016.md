## `adoptopenjdk:11-hotspot-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:c8f5bc57d1e790701183a23cc7f220928df508e32a3296b78a8d9d5364206d89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `adoptopenjdk:11-hotspot-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull adoptopenjdk@sha256:b857f431b8e3c30dad5c8e6edaba28d26d91d9e05f6362f3657f6cf1a2e9391d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 GB (6634012754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:951b0eee9bd9ba467af54435e6b6bace38af58fa17f3a4b812555327dde3393a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:35:32 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Wed, 14 Jul 2021 15:37:57 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.11_9.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12 ; Invoke-WebRequest -Uri https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.11_9.msi -O 'openjdk.msi' ;     Write-Host ('Verifying sha256 (de7de70fbd9f3ff49ce34db87c5f331a5c0b72e54c16e9e6d9ba3007d23b361e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'de7de70fbd9f3ff49ce34db87c5f331a5c0b72e54c16e9e6d9ba3007d23b361e') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jul 2021 15:38:00 GMT
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
	-	`sha256:cbb71621f9cd98b7ad71021e44b018da3eb9b1e275ad0d9d6aab8b096d56ff24`  
		Last Modified: Wed, 14 Jul 2021 16:51:47 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50536af40905c39c21f5a87f1e4dea96a08ef0b653282482e798f9ab97c347dc`  
		Last Modified: Wed, 14 Jul 2021 16:52:16 GMT  
		Size: 364.4 MB (364376513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3d83244dec54be0c077c1c7dfbad4126360bdd03f9b0f0fa0a1869fa688749`  
		Last Modified: Wed, 14 Jul 2021 16:51:47 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
