## `adoptopenjdk:14-jre-openj9-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:c628f3f8a7df65e787f89a84ba57d18402cb355ef98d3be13c69d3b3f788db05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `adoptopenjdk:14-jre-openj9-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull adoptopenjdk@sha256:3575072a5ecea3549eb4b16b6b536b0e3184eddce7883b79b7fb0a6564c65922
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819652765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90daa9bc9df9e59afaf014ad9ea99bf628f91fe0c5b3c968421275414f720199`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Apr 2020 17:55:32 GMT
ENV JAVA_VERSION=jdk-14.0.1+7_openj9-0.20.0
# Mon, 20 Apr 2020 18:04:21 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7_openj9-0.20.0/OpenJDK14U-jre_x64_windows_openj9_14.0.1_7_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7_openj9-0.20.0/OpenJDK14U-jre_x64_windows_openj9_14.0.1_7_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (086a64997988dbfa5dbbfa9656b0c9d41c651f94b600fc01fdb3bc2c09b807e6) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '086a64997988dbfa5dbbfa9656b0c9d41c651f94b600fc01fdb3bc2c09b807e6') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Mon, 20 Apr 2020 18:04:22 GMT
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
	-	`sha256:300e5ee7c8921d26d1a59365c4fecd5f1fa99a0e6744b2b1c6fd80c32c2d5c9f`  
		Last Modified: Mon, 20 Apr 2020 18:18:39 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9896875101f379dcda6cf59eacbec728389f5239be37bb408d997c81ee08c8eb`  
		Last Modified: Mon, 20 Apr 2020 18:22:47 GMT  
		Size: 91.6 MB (91581787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93922c08622cdff16fe316af2f49cd5bdc55c384d3af2a298a324ad20d283f9`  
		Last Modified: Mon, 20 Apr 2020 18:21:11 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:14-jre-openj9-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull adoptopenjdk@sha256:4e0cf862e8a95e61b474dbe8874242a3115c7bfe128aa609215cc7bb5f30f80a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2361641760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55898a55c725853775c836f26022b3f91de5c5ab826d9feed8c5ec902401c3fa`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Apr 2020 17:59:14 GMT
ENV JAVA_VERSION=jdk-14.0.1+7_openj9-0.20.0
# Mon, 20 Apr 2020 18:05:58 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7_openj9-0.20.0/OpenJDK14U-jre_x64_windows_openj9_14.0.1_7_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7_openj9-0.20.0/OpenJDK14U-jre_x64_windows_openj9_14.0.1_7_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (086a64997988dbfa5dbbfa9656b0c9d41c651f94b600fc01fdb3bc2c09b807e6) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '086a64997988dbfa5dbbfa9656b0c9d41c651f94b600fc01fdb3bc2c09b807e6') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Mon, 20 Apr 2020 18:05:59 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edc29de224149bd438350512f7a31a67edbd3fcafce757aa60620dc459c184ad`  
		Last Modified: Tue, 14 Apr 2020 22:15:56 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b506f9f49cb96c23ac8085528a8f84e9e9ba28daa97d4338305b90e9d4f83af8`  
		Last Modified: Mon, 20 Apr 2020 18:19:33 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829e3ed8b277f72c0c3bad50f66db7cae053699beac7681b311874cfab6cae75`  
		Last Modified: Mon, 20 Apr 2020 18:23:10 GMT  
		Size: 90.9 MB (90931145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb53a3ed5cfc6afd4e900997164be13f92084c5b1beec6bb4caae727626ecb27`  
		Last Modified: Mon, 20 Apr 2020 18:22:57 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
