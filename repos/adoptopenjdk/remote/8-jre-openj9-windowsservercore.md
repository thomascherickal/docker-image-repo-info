## `adoptopenjdk:8-jre-openj9-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:8aa078b5fabb05b9bb13d1ca1c7342d5d472add59757cb00ed3752c981e3c99e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `adoptopenjdk:8-jre-openj9-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull adoptopenjdk@sha256:ce2c4f23cf6cd9ff300bff14e23ca503b3f861137240fb5d94a8809340059db9
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5821146357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd8109621422889490c38437212280a56b7fcb302c920553c6f118ea5c75f52`
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
# Mon, 20 Apr 2020 17:43:29 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_windows_openj9_8u252b09_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_windows_openj9_8u252b09_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (ea7bf4e3386d650ef60118dc9fb077e4f4c2ad57e774c495cefdd59dcea476ac) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'ea7bf4e3386d650ef60118dc9fb077e4f4c2ad57e774c495cefdd59dcea476ac') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Mon, 20 Apr 2020 17:43:30 GMT
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
	-	`sha256:f9095ad3811b9d8593e44fdee0d2876975fc31558ed6307c78ca91da1b95d7e1`  
		Last Modified: Mon, 20 Apr 2020 18:15:26 GMT  
		Size: 93.1 MB (93075344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b49ab94fe1250619c3e38ff2cee54fecd8cde49eceedaffed0a2ed79500328`  
		Last Modified: Mon, 20 Apr 2020 18:15:14 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:8-jre-openj9-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull adoptopenjdk@sha256:87792c75a1daade9ffb54bd5d98db366e96f9229cc7aebd755a9c8dab5eedf47
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363137755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a8fac2b7ce0bf83cc2f1fc992975574393d36d96a6b706053eff8a8814de83`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Apr 2020 17:39:23 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Mon, 20 Apr 2020 17:45:06 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_windows_openj9_8u252b09_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_windows_openj9_8u252b09_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (ea7bf4e3386d650ef60118dc9fb077e4f4c2ad57e774c495cefdd59dcea476ac) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'ea7bf4e3386d650ef60118dc9fb077e4f4c2ad57e774c495cefdd59dcea476ac') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Mon, 20 Apr 2020 17:45:08 GMT
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
	-	`sha256:c9e84764eb3971bda1b806fe366008f8c4f3379bf29022d305f2e2e68bb70092`  
		Last Modified: Mon, 20 Apr 2020 18:10:45 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7755421850feab973489ba6ffae460b6f78b0bfbf0666c2b8b7b05a8b98eebc`  
		Last Modified: Mon, 20 Apr 2020 18:15:48 GMT  
		Size: 92.4 MB (92427089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9721823ba9b515f6622c0cec76379554d72ec3fdb354e11c0a44ebad8c9161`  
		Last Modified: Mon, 20 Apr 2020 18:15:38 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
