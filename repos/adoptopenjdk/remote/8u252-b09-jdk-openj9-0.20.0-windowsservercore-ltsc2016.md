## `adoptopenjdk:8u252-b09-jdk-openj9-0.20.0-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:6c61a6d5f0033983d3ddfb134e50a78437d78f4836c2d0d71102490b8706d234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `adoptopenjdk:8u252-b09-jdk-openj9-0.20.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull adoptopenjdk@sha256:5544519411fcd3973dcfdd8ffe814de0a928aca3f54e06c9c08a24385e11b442
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5952636224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07aaa80f372e507e2d17595290f1fb81e674bf674aeaf8bc5840cf0e76ecc4dd`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Apr 2020 17:35:24 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 20 Apr 2020 17:39:15 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jdk_x64_windows_openj9_8u252b09_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jdk_x64_windows_openj9_8u252b09_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (5e41cb4f33b4a605f87275e4830514db20dad053cb7b5dd52bd73143abc2c7d3) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '5e41cb4f33b4a605f87275e4830514db20dad053cb7b5dd52bd73143abc2c7d3') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Mon, 20 Apr 2020 17:39:16 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ac0134cee91589d04e97f11994235cce86faef5c581d15f2e143ecb90e92572`  
		Last Modified: Tue, 14 Apr 2020 22:16:36 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9ffea01a81e41ed9a00d68c52ffad2ff9d1d165e366607dc5d416127e76513`  
		Last Modified: Mon, 20 Apr 2020 18:09:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcdcb8d742f224dec90589199bf2e84575fd4fae0c4f6b93aeda959fe9cd4aa`  
		Last Modified: Mon, 20 Apr 2020 18:10:21 GMT  
		Size: 224.6 MB (224565225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6632dcabff12051292da1b18c56d92cb8944c102e6353a8959d760f6ac52db60`  
		Last Modified: Mon, 20 Apr 2020 18:09:59 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
