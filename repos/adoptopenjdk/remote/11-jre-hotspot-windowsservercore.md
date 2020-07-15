## `adoptopenjdk:11-jre-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:e39b57b91b62074adc3778ced0032d2a39c332bb5180baad481f7b89ab75c6c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3808; amd64
	-	windows version 10.0.17763.1339; amd64

### `adoptopenjdk:11-jre-hotspot-windowsservercore` - windows version 10.0.14393.3808; amd64

```console
$ docker pull adoptopenjdk@sha256:63f29752a9eb399040a0ee7e780a1ce03e76fc88d59b1142badac5d8f33efd1b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5818602595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb990c02eec347cc2b3535247c63e81fc506b4d9faaf45493d85ea733c8e8a6c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Jul 2020 21:05:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 14 Jul 2020 18:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 18:45:12 GMT
ENV JAVA_VERSION=jdk-11.0.7+10.2
# Wed, 15 Jul 2020 18:54:04 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10.2/OpenJDK11U-jre_x64_windows_hotspot_11.0.7_10.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10.2/OpenJDK11U-jre_x64_windows_hotspot_11.0.7_10.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (0d3d85adb69ad01eb77a26347a23b8ac62f27ee2d3d7bacb401faf9b89d3c4a8) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '0d3d85adb69ad01eb77a26347a23b8ac62f27ee2d3d7bacb401faf9b89d3c4a8') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:802c4beb8b091968ccf1bb4a853ded7955ddb79e6f8775a5155cb5ed07dcbcab`  
		Size: 1.7 GB (1667476199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9a64f8d0454dba1fb133615caae6ab4d76b85b8be54102ee2ce5f7fd034edbff`  
		Last Modified: Tue, 14 Jul 2020 19:42:07 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c33a8359f8a5153ef340fb72363fef91f5b6e0696eebf0ff78c115c7b198df`  
		Last Modified: Wed, 15 Jul 2020 20:08:13 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622cf89ec3e28d25468c854f004693a810ea46cc4c60b167a1dc8d7fb4609640`  
		Last Modified: Wed, 15 Jul 2020 20:09:57 GMT  
		Size: 81.1 MB (81138237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:11-jre-hotspot-windowsservercore` - windows version 10.0.17763.1339; amd64

```console
$ docker pull adoptopenjdk@sha256:9b05d0610bc4680b54f914fcdcfb96f38e2fcc30b444b6d614e778bc19995fd5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2390694564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c15d52d67f3c831c8978aef2ac1280bea5e1465834c35140d10bacb874fc5925`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jul 2020 18:48:54 GMT
ENV JAVA_VERSION=jdk-11.0.7+10.2
# Wed, 15 Jul 2020 18:55:47 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10.2/OpenJDK11U-jre_x64_windows_hotspot_11.0.7_10.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.7%2B10.2/OpenJDK11U-jre_x64_windows_hotspot_11.0.7_10.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (0d3d85adb69ad01eb77a26347a23b8ac62f27ee2d3d7bacb401faf9b89d3c4a8) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '0d3d85adb69ad01eb77a26347a23b8ac62f27ee2d3d7bacb401faf9b89d3c4a8') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72d212a8d1af1a4d7690db93272df429379d0e6aaa4ee45549a872cf48d2bce`  
		Last Modified: Wed, 15 Jul 2020 20:08:58 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b190f2da62f34341efe808a75b91bcbb573de5e6bc6844d19fd673e32492389`  
		Last Modified: Wed, 15 Jul 2020 20:10:20 GMT  
		Size: 80.5 MB (80500023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
