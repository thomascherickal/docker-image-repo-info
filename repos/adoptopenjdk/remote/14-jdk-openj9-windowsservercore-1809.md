## `adoptopenjdk:14-jdk-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:fd6b0141573dc868e87f66cb0ab3c05757c02b174504988380df47d9cdecba17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `adoptopenjdk:14-jdk-openj9-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull adoptopenjdk@sha256:375b1ab0580082f969c962c220e40bcf0b0e06903a3877e6505d1401cea2ab09
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2658291862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f5a5813093b1b510591f5fdaed6880b9f8d01ecc291144c7a46868257cf3317`
-	Default Command: `["jshell"]`
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
# Mon, 20 Apr 2020 18:01:53 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7_openj9-0.20.0/OpenJDK14U-jdk_x64_windows_openj9_14.0.1_7_openj9-0.20.0.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7_openj9-0.20.0/OpenJDK14U-jdk_x64_windows_openj9_14.0.1_7_openj9-0.20.0.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (49304cd0d37bd6c62d519246899f5e067651dfa328f60a91e92f96ba01831e40) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '49304cd0d37bd6c62d519246899f5e067651dfa328f60a91e92f96ba01831e40') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Mon, 20 Apr 2020 18:01:55 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Mon, 20 Apr 2020 18:01:56 GMT
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
	-	`sha256:b506f9f49cb96c23ac8085528a8f84e9e9ba28daa97d4338305b90e9d4f83af8`  
		Last Modified: Mon, 20 Apr 2020 18:19:33 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07e6fadb3d5d14682c088327d53ba155fdd93dbee4b70564084e540bc2e0682`  
		Last Modified: Mon, 20 Apr 2020 18:20:54 GMT  
		Size: 387.6 MB (387580069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a556c198347285319eb548a493c17485edb54c879e29fcfc1c3f28ee7df8d9cb`  
		Last Modified: Mon, 20 Apr 2020 18:19:33 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f971b64be84f43410d5273d1563fdf613f8eb8d02619a838342c9767fc2634`  
		Last Modified: Mon, 20 Apr 2020 18:19:33 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
