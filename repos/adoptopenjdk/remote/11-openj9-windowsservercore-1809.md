## `adoptopenjdk:11-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:167fd9e01bb5dc963e8016b2ba54d644321cbbcfd7da6b963bd717823065c119
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `adoptopenjdk:11-openj9-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull adoptopenjdk@sha256:de5b950c6b5223d6760ae248ddcb07a61886fe194d43579ddeda20bb5c382fb7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2815232297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb6e22fd9afab6ec27a56143cb276d455a7ad85187c31c060d2e2214c0c30d08`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 22:34:10 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 13 Jan 2021 22:36:39 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.9_11_openj9-0.23.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.9_11_openj9-0.23.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (c4885100b0565a63dc3e21a47c6e344ea863ec533d67664e06494385c5923cb3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'c4885100b0565a63dc3e21a47c6e344ea863ec533d67664e06494385c5923cb3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Jan 2021 22:36:40 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 13 Jan 2021 22:36:41 GMT
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
	-	`sha256:0306996a905cb58d790e9a7140aabce8dcf2576ba4a8548b412370c82398a6ad`  
		Last Modified: Wed, 13 Jan 2021 23:32:43 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71a7eadf416c8d0245189e4b64e9698310fa4309b50fc1e2ed7b324bbf4bf27`  
		Last Modified: Wed, 13 Jan 2021 23:33:14 GMT  
		Size: 379.5 MB (379455680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f62b966def4c4e0d6beb61129e697459d5ffc27f73816b403165fef5b0abdc`  
		Last Modified: Wed, 13 Jan 2021 23:32:42 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5104c90b822eb20c36f9aa18721f2189b1ca558c555f80ff3bc95402fd08b08b`  
		Last Modified: Wed, 13 Jan 2021 23:32:42 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
