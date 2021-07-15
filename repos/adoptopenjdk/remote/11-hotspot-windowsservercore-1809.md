## `adoptopenjdk:11-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:f897b9d4e341e470c5f0d3f25b26683cffaf42123d3027fbbaa36741e1eae46a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `adoptopenjdk:11-hotspot-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull adoptopenjdk@sha256:7224d3a39dfdb53cf2ce21f956443731c97584daa904089a016861bdc102ab7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 GB (3049898033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8edae840009f5ce2aad6f3284d3f78458bab3d7b699fb2bc80d623b3087a3554`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 15:33:20 GMT
ENV JAVA_VERSION=jdk-11.0.11+9
# Wed, 14 Jul 2021 15:35:09 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.11_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.11_9.msi ;     Write-Host ('Verifying sha256 (de7de70fbd9f3ff49ce34db87c5f331a5c0b72e54c16e9e6d9ba3007d23b361e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'de7de70fbd9f3ff49ce34db87c5f331a5c0b72e54c16e9e6d9ba3007d23b361e') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Jul 2021 15:35:12 GMT
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
	-	`sha256:f047fbbd8b17018ca409212e52b95f4daaa10861fcfc86be53d143948858be80`  
		Last Modified: Wed, 14 Jul 2021 16:44:10 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756978c476bcdc8f329602460b6c2ccbffe0c8295aa70b88d6fe05d5cc36b006`  
		Last Modified: Wed, 14 Jul 2021 16:51:33 GMT  
		Size: 364.4 MB (364446945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012f664205c3ea7ba0773800f93a2e48938a31d4a76beb4200716af14c6cad22`  
		Last Modified: Wed, 14 Jul 2021 16:44:10 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
