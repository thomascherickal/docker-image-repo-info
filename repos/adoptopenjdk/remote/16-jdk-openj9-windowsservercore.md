## `adoptopenjdk:16-jdk-openj9-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:e88908f3fd3ba941baeab1337322dd232159562aee0937e459fc6030bcd0f705
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `adoptopenjdk:16-jdk-openj9-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull adoptopenjdk@sha256:01d1043392e4140f4d693a6d18f4b365feca462ea8a61ac428e2dbc5eaa853e9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2865881852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:664c9fc429204a13b198a0fb8f399023159da9010115de573e926b2d40af1828`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 19:00:56 GMT
ENV JAVA_VERSION=jdk-16+36_openj9-0.25.0
# Wed, 14 Apr 2021 19:02:46 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36_openj9-0.25.0/OpenJDK16-jdk_x64_windows_openj9_16_36_openj9-0.25.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36_openj9-0.25.0/OpenJDK16-jdk_x64_windows_openj9_16_36_openj9-0.25.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (5d5a2dd21567b376185076c4fcba42caf9e5c35565bbc2c416140514c8622460) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '5d5a2dd21567b376185076c4fcba42caf9e5c35565bbc2c416140514c8622460') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Apr 2021 19:02:47 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 14 Apr 2021 19:02:48 GMT
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
	-	`sha256:939c85804a327c9fbbf04531f81abe1f87370c9381114f168c60d227babb015d`  
		Last Modified: Wed, 14 Apr 2021 19:42:43 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe62b85759647063426cf0bc42892b62b28114d463c8baf757da6dbe3e1da08`  
		Last Modified: Wed, 14 Apr 2021 19:49:54 GMT  
		Size: 396.1 MB (396122317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdb5368fe2589d337cc8e5ff7cef4bf537db0f0abda62c1194c49b9aaf7fa39`  
		Last Modified: Wed, 14 Apr 2021 19:42:43 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d452e4371bb2983f20561539736d30422d2be458f367ad38e921ffcb3731b1`  
		Last Modified: Wed, 14 Apr 2021 19:42:43 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16-jdk-openj9-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull adoptopenjdk@sha256:d4b71f7bc0aad84e11e37003a824bd53d1763310339fe8515f8a9a03a032ec0a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6196025689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b7968e7fe08d97e2fe2a1d4e74bdccb5d0e62e4b16a1090640d0aec59d820d1`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 19:02:58 GMT
ENV JAVA_VERSION=jdk-16+36_openj9-0.25.0
# Wed, 14 Apr 2021 19:05:34 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36_openj9-0.25.0/OpenJDK16-jdk_x64_windows_openj9_16_36_openj9-0.25.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36_openj9-0.25.0/OpenJDK16-jdk_x64_windows_openj9_16_36_openj9-0.25.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (5d5a2dd21567b376185076c4fcba42caf9e5c35565bbc2c416140514c8622460) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '5d5a2dd21567b376185076c4fcba42caf9e5c35565bbc2c416140514c8622460') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Apr 2021 19:05:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 14 Apr 2021 19:05:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91c7a604fa3bb5d849a227e9d5a853b5b4a28f31d9533b1d7d85cd45e5d01bf`  
		Last Modified: Wed, 14 Apr 2021 19:50:17 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645a36a71fb4d0ac2c4cb72e23a048abd69f18f9c533844555d65f355bc3c15a`  
		Last Modified: Wed, 14 Apr 2021 19:57:42 GMT  
		Size: 401.1 MB (401136123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6e98b21f1b2961761c74d55525a7bf8a42e4b0a0792f88453da266df69f8e3`  
		Last Modified: Wed, 14 Apr 2021 19:50:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b2e6dfbf781be1427972ea448f03165a18acf2b421a14f743cd4c8a8384851`  
		Last Modified: Wed, 14 Apr 2021 19:50:18 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
