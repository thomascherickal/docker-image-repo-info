## `adoptopenjdk:11-jdk-openj9-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:51f02f2c119a9abf6e2c96f481b46da6a7b457889ff6377c4c6a82d929022b9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `adoptopenjdk:11-jdk-openj9-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull adoptopenjdk@sha256:2199acca27381887ac6df674ca53f57571cd8b263a526ba34a73a41a91479244
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6110002920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aac80d8c2668dbfd2e6150a28acf1ceaad46d97629b901cb5f5328ee5a83aca0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 12:34:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 17:18:56 GMT
ENV JAVA_VERSION=jdk-11.0.7+10.1_openj9-0.20.0
# Wed, 13 May 2020 17:22:12 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10.1_openj9-0.20.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.7_10_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10.1_openj9-0.20.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.7_10_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (386e33d5b3bb9ed01b3b96e4d68933cc50d87deca7cfbdc8d360929340de16d5) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '386e33d5b3bb9ed01b3b96e4d68933cc50d87deca7cfbdc8d360929340de16d5') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Wed, 13 May 2020 17:22:13 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 13 May 2020 17:22:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e3e9730c43354781e87aa51e853bff3b1e8c1ca7004f527139638a8f9d499c49`  
		Last Modified: Wed, 13 May 2020 12:59:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ec8ec7d0b4ed8a93263033a2dc6913b00ad96451635f34759a2237004e7c84`  
		Last Modified: Wed, 13 May 2020 18:27:06 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d3d1d55dda403d7e2d8a5eb9bc87964bbc9590bb10d9e8b02da5955baca6be`  
		Last Modified: Wed, 13 May 2020 18:28:20 GMT  
		Size: 378.1 MB (378108484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233cd44a1c6e33371acfcefad7a4ef8fa0568eeafc1a4100cdecc79d24b339f1`  
		Last Modified: Wed, 13 May 2020 18:27:06 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ef1145f4c4d4b6e8851079c19d612177fbfdda75b9b24eb5b1dc4f1693b36c`  
		Last Modified: Wed, 13 May 2020 18:27:06 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jdk-openj9-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull adoptopenjdk@sha256:bc64b7bf08f9e58243602423a84f8cb4867cab00689d946135ada00556a4bf73
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086967030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e280c202f2cff98d0936f2bb56a8771af723ca2ac7e3b299ac7b25fe289b349`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 12:41:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 17:22:22 GMT
ENV JAVA_VERSION=jdk-11.0.7+10.1_openj9-0.20.0
# Wed, 13 May 2020 17:24:39 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10.1_openj9-0.20.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.7_10_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10.1_openj9-0.20.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.7_10_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (386e33d5b3bb9ed01b3b96e4d68933cc50d87deca7cfbdc8d360929340de16d5) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '386e33d5b3bb9ed01b3b96e4d68933cc50d87deca7cfbdc8d360929340de16d5') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Wed, 13 May 2020 17:24:41 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 13 May 2020 17:24:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:77613e754ba9d62c0acd4ef271c4ee7d3af091b8c8b310afa404560a9d281f82`  
		Last Modified: Wed, 13 May 2020 13:00:20 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d810ccd15d7c31a36ee65ea8b587f5efb4eec16a8c827e6476ab4036a37f93`  
		Last Modified: Wed, 13 May 2020 18:28:34 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0262b4f588772db19f66780173074944e1afbfab36d8223ff7a7f2cdb6adba`  
		Last Modified: Wed, 13 May 2020 18:34:54 GMT  
		Size: 368.6 MB (368629556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc003d081f08a663961438d7b6d5731da07f15987e14f9235ace859cd1f87535`  
		Last Modified: Wed, 13 May 2020 18:28:34 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2b645642d2d842af7cb64241499b9e58acb1cf83b9bed0f209088345265417`  
		Last Modified: Wed, 13 May 2020 18:28:35 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
