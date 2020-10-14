## `adoptopenjdk:hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:59643524640b702f3784b8eb25752bd8baa31a8c0001d53bd8a3d062cd0d0745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64
	-	windows version 10.0.17763.1518; amd64

### `adoptopenjdk:hotspot-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull adoptopenjdk@sha256:e478d85af2e3d3ec954920890f67b7b3dc4057428c6b6cc6d710dfa313847fad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6142137181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7cffd981a6fb2719d68b6e253adafa63e5a2be6349ddcaab382e5643f0ce91`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 19:17:36 GMT
ENV JAVA_VERSION=jdk-13.0.2+8
# Wed, 14 Oct 2020 19:21:02 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jdk_x64_windows_hotspot_13.0.2_8.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jdk_x64_windows_hotspot_13.0.2_8.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (422a4ce0668df53cd891ea38e6c472941893b26c9eb4121787d7c1eee123abee) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '422a4ce0668df53cd891ea38e6c472941893b26c9eb4121787d7c1eee123abee') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Wed, 14 Oct 2020 19:21:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f179e6010a33d7aebcdcd3e436752c9334bba084851fac1b9283a4a79da38562`  
		Last Modified: Wed, 14 Oct 2020 20:26:17 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f7405c7800a5e07ea7ef48f2fca4a374021fecd6b3fee2a8f3f946e54eab85`  
		Last Modified: Wed, 14 Oct 2020 20:27:00 GMT  
		Size: 400.8 MB (400782099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ff0add9481ff0bddd18ce9627812663c53648354f44541fa8e05e4e336f0ff`  
		Last Modified: Wed, 14 Oct 2020 20:26:17 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:hotspot-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:0478f0b476640e61570a7436e2a29803e4629f59d9706d234ccbcf276d47fddf
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2774245948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5be204018b5dafb4715017fa2eef0bdbc4affb467ccca1aafe01b6a66cfcbf89`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 19:21:18 GMT
ENV JAVA_VERSION=jdk-13.0.2+8
# Wed, 14 Oct 2020 19:23:58 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jdk_x64_windows_hotspot_13.0.2_8.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk13-binaries/releases/download/jdk-13.0.2%2B8/OpenJDK13U-jdk_x64_windows_hotspot_13.0.2_8.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (422a4ce0668df53cd891ea38e6c472941893b26c9eb4121787d7c1eee123abee) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '422a4ce0668df53cd891ea38e6c472941893b26c9eb4121787d7c1eee123abee') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
# Wed, 14 Oct 2020 19:23:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda0d178e1807a31e12cc6c7546057f97c77bb40223ea71f9e459399601e0087`  
		Last Modified: Wed, 14 Oct 2020 20:27:17 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951de98c2f62083e2dc4a2ac5f69850ece7bcc4410f9f2f6731936e153f40c73`  
		Last Modified: Wed, 14 Oct 2020 20:28:02 GMT  
		Size: 400.2 MB (400152403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdceed887c933d53c57881d1fbfb4548bd6ed60b55a0128d372fdd42683b04cb`  
		Last Modified: Wed, 14 Oct 2020 20:27:17 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:hotspot-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull adoptopenjdk@sha256:e696907269da825807b5683b79d50ee43272579f01442ed24418ebe955f904c7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6136397482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a565c95fe36f4ee89bdd50d1f24bf57bc997df4d4870a5c43ede0c59e18adbf6`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 19:28:08 GMT
ENV JAVA_VERSION=jdk-14.0.2+12
# Wed, 14 Oct 2020 19:31:27 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_x64_windows_hotspot_14.0.2_12.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_x64_windows_hotspot_14.0.2_12.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (9cbd03600e58ad8d2383c15e596396fbdfbc9655ba0019f5bc74c910e4082c7c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '9cbd03600e58ad8d2383c15e596396fbdfbc9655ba0019f5bc74c910e4082c7c') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Oct 2020 19:31:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3685603ccf52c648bccad78e97a5b2519fb7c160445169e7e0ce6d9a47950d79`  
		Last Modified: Wed, 14 Oct 2020 20:29:12 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a0ba07380ff0a636a064b7397896b2f8c85e4932506f7ed0e8f6821d7764fa`  
		Last Modified: Wed, 14 Oct 2020 20:29:49 GMT  
		Size: 395.0 MB (395042401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83767a65fce2b8b813b60bb21a44c04ff503a81d14cfa6360544cca78ce9dafe`  
		Last Modified: Wed, 14 Oct 2020 20:29:12 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:hotspot-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:b6497f8839fb985c905d0f2f33ac193bc426419287ad7de398f5b53d6814338b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2768498205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3f09ffcde7f33639f893134cb6e8e7569fa9705dc678d76443ef37cbc51c0e0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Oct 2020 19:31:35 GMT
ENV JAVA_VERSION=jdk-14.0.2+12
# Wed, 14 Oct 2020 19:34:13 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_x64_windows_hotspot_14.0.2_12.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.2%2B12/OpenJDK14U-jdk_x64_windows_hotspot_14.0.2_12.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (9cbd03600e58ad8d2383c15e596396fbdfbc9655ba0019f5bc74c910e4082c7c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '9cbd03600e58ad8d2383c15e596396fbdfbc9655ba0019f5bc74c910e4082c7c') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 14 Oct 2020 19:34:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6603c30dfb6ece9de47b2967f87b8170d294e61de2afd3ea6d5fac51dd9b9ea`  
		Last Modified: Wed, 14 Oct 2020 20:30:11 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c534f0b6571cf97d7e0992a60901129600f5f0e70814ddbe583679202214ce26`  
		Last Modified: Wed, 14 Oct 2020 20:30:44 GMT  
		Size: 394.4 MB (394404676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1605d2deb85ecf5994b6a620370a6506231023c0d3020ca636a662b72f47ef83`  
		Last Modified: Wed, 14 Oct 2020 20:30:11 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
