## `adoptopenjdk:16-jre-openj9-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:44b5586fbd4d902ee1add3fee02a39c86f385c6d0e92316e985a1cece6ac002c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `adoptopenjdk:16-jre-openj9-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull adoptopenjdk@sha256:1261181ac4575be28a20063f8c24f487cc20af858d10a363bb7a7fa53a5851cf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2548488685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d56996a0d45422bb0d25cafb740aad48376c65c8261db58a8a4982223001838`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 14 Apr 2021 19:07:11 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36_openj9-0.25.0/OpenJDK16-jre_x64_windows_openj9_16_36_openj9-0.25.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36_openj9-0.25.0/OpenJDK16-jre_x64_windows_openj9_16_36_openj9-0.25.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (49e6a468a50b65f7b3839881bca7a7fbea1be81d734f1b52662063a6db563387) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '49e6a468a50b65f7b3839881bca7a7fbea1be81d734f1b52662063a6db563387') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Apr 2021 19:07:12 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
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
	-	`sha256:a192c7527a7c3bacca936ea396a3217bade448522cc6fd435035fce34a26c5d1`  
		Last Modified: Wed, 14 Apr 2021 19:58:11 GMT  
		Size: 78.7 MB (78730550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f1b0c9b9e90826fd2285479e4fd05dca802c02ffbfa0e28c888f5ed4fefe51`  
		Last Modified: Wed, 14 Apr 2021 19:57:59 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:16-jre-openj9-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull adoptopenjdk@sha256:b2336d4723b106423e2b4f44df6b18203ec29927b2c0882143404961ec6a2b72
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5874136954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06573014429efb6f8f5f58b491659772e9298d0cc8561f501f5ffd81ccb81a5f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 14 Apr 2021 19:09:25 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36_openj9-0.25.0/OpenJDK16-jre_x64_windows_openj9_16_36_openj9-0.25.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16%2B36_openj9-0.25.0/OpenJDK16-jre_x64_windows_openj9_16_36_openj9-0.25.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (49e6a468a50b65f7b3839881bca7a7fbea1be81d734f1b52662063a6db563387) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '49e6a468a50b65f7b3839881bca7a7fbea1be81d734f1b52662063a6db563387') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Apr 2021 19:09:26 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
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
	-	`sha256:14c658b17f97b371a590ea6fbebe4192211996299511c9cf96487ada387fcb5d`  
		Last Modified: Wed, 14 Apr 2021 19:58:35 GMT  
		Size: 79.2 MB (79248826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec1a6de85e6390aea467406dac35190b64e7be1efc0f9fcb69a67a8663ef2aa`  
		Last Modified: Wed, 14 Apr 2021 19:58:23 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
