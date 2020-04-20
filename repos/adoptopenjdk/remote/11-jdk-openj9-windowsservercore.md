## `adoptopenjdk:11-jdk-openj9-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:2a0865ae425899fbb376394e285a0f44dd4b6e26fa4d0fbad176d1643acb7fef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `adoptopenjdk:11-jdk-openj9-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull adoptopenjdk@sha256:db7f7d7c123f530c5649415d1d280a37aa48f23ca911c636938ad7092c02fd5a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6105954039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa1c89b0d5cd4718eafcabad0a9c57277a97accab1427673a5025e63907b812f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Apr 2020 21:35:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Apr 2020 17:45:26 GMT
ENV JAVA_VERSION=jdk-11.0.7+10_openj9-0.20.0
# Mon, 20 Apr 2020 17:48:47 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10_openj9-0.20.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.7_10_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10_openj9-0.20.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.7_10_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (8d5736b42b16261bf8a74e6126890b8032dd08d9c7095d5b5484708f3dec2a72) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8d5736b42b16261bf8a74e6126890b8032dd08d9c7095d5b5484708f3dec2a72') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Mon, 20 Apr 2020 17:48:49 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 20 Apr 2020 17:48:50 GMT
CMD ["jshell"]
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
	-	`sha256:2fb46dd1e5ab3f79811729cc3487559cdcbcfe529cd65624ceb5a0c337475fba`  
		Last Modified: Mon, 20 Apr 2020 18:15:58 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca3cb99ca9b60bb074f13baa50f14c6e6043bfbcfeed2e9335bab837d4231f`  
		Last Modified: Mon, 20 Apr 2020 18:16:31 GMT  
		Size: 377.9 MB (377881914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caad3dff5cfaa6a45ab68411963f25379c9a6db367421dbeab0cf0423496f67d`  
		Last Modified: Mon, 20 Apr 2020 18:15:58 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b554f66f25be5776bb80040ba8781e244112b4754bfae1e19f03d21bbaddc53`  
		Last Modified: Mon, 20 Apr 2020 18:15:59 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jdk-openj9-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull adoptopenjdk@sha256:c760c40410bbf9e7905fb51e695908547b45ec69718c7ead4be9430bbf411b83
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2643429106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3212e74677a972adf2ec0b70886f0a58b525a81aaf9aa4b95bff8786cf4386a9`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Tue, 14 Apr 2020 21:32:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 20 Apr 2020 17:49:08 GMT
ENV JAVA_VERSION=jdk-11.0.7+10_openj9-0.20.0
# Mon, 20 Apr 2020 17:51:43 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10_openj9-0.20.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.7_10_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10_openj9-0.20.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.7_10_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (8d5736b42b16261bf8a74e6126890b8032dd08d9c7095d5b5484708f3dec2a72) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '8d5736b42b16261bf8a74e6126890b8032dd08d9c7095d5b5484708f3dec2a72') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Mon, 20 Apr 2020 17:51:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 20 Apr 2020 17:51:45 GMT
CMD ["jshell"]
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
	-	`sha256:963d6a2e0981d9b6a994ccdc70eac22c8cbc3d9ea90e55dd36791d3522a8e75d`  
		Last Modified: Mon, 20 Apr 2020 18:17:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c7d94db0f21c0471fbb8c003af60fec3bb3dfa3568d5b76ab9bcab0b549c96`  
		Last Modified: Mon, 20 Apr 2020 18:17:42 GMT  
		Size: 372.7 MB (372717340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8616d98ab3231f72b62fd0b5c5949b890ce12c34c34cc45cc0d7cdc208e6f1d4`  
		Last Modified: Mon, 20 Apr 2020 18:17:13 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741a71f8f677e01aafca7b621a87917de47fae009f9061e65ae13442f8382eaa`  
		Last Modified: Mon, 20 Apr 2020 18:17:13 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
