## `adoptopenjdk:15-jdk-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:b5dcd51a610b9d2834b756a6b93aa582d941e9f0d6888fbbadcbcea822941ed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `adoptopenjdk:15-jdk-hotspot-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull adoptopenjdk@sha256:65aae9c76512e99f32a4db0cdbcc9b09207043805bd977f37dfe38e546114022
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2768445684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a67d4d1e8a706c3e041137d4715f31a6d5d5268325ddb9e4b2cd71384ab8937`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 20:50:52 GMT
ENV JAVA_VERSION=jdk-15.0.1+9
# Wed, 09 Dec 2020 20:53:23 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_windows_hotspot_15.0.1_9.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_windows_hotspot_15.0.1_9.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (7254fbe32e77a6cb8c6e36fd1da8ee0744fb323addb0bfda4c32a4d6cf9d22ce) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '7254fbe32e77a6cb8c6e36fd1da8ee0744fb323addb0bfda4c32a4d6cf9d22ce') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 20:53:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f605bfaef97583fdcbe31c01f8f9e07a288b149c3bec939c932450ac9b470bd`  
		Last Modified: Wed, 09 Dec 2020 21:52:43 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f502c185c80c4a8fdb1c7fe01ea0446485af21dca655a179547e3c58067255`  
		Last Modified: Wed, 09 Dec 2020 21:53:13 GMT  
		Size: 377.6 MB (377567793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af08a159eff74a5b8c07695e7d46c206bcf02adf7238d1a51f489a8ba1a1036d`  
		Last Modified: Wed, 09 Dec 2020 21:52:44 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jdk-hotspot-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull adoptopenjdk@sha256:ec8489079184b11414eba63812123f8c40a51a0833ade608d0ab9b6c4065a63d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6147170818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b03f5bea35f377c0237755a72771f85b84efed164af76b250d1da5a05d891632`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 20:53:33 GMT
ENV JAVA_VERSION=jdk-15.0.1+9
# Wed, 09 Dec 2020 20:56:48 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_windows_hotspot_15.0.1_9.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9/OpenJDK15U-jdk_x64_windows_hotspot_15.0.1_9.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (7254fbe32e77a6cb8c6e36fd1da8ee0744fb323addb0bfda4c32a4d6cf9d22ce) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '7254fbe32e77a6cb8c6e36fd1da8ee0744fb323addb0bfda4c32a4d6cf9d22ce') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 20:56:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed279ee84bb22c7ab5cb559bff57272a4ccd9a60ad3255fec03f0ae21a8f8a3b`  
		Last Modified: Wed, 09 Dec 2020 21:53:33 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71356dfc927d9c078512eefa8d6f11eaaa2b03cc491c13efa1adec9f6f54a36`  
		Last Modified: Wed, 09 Dec 2020 21:54:03 GMT  
		Size: 378.3 MB (378323357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730910424615cf1ec0e906e156fa9e9f5c6fdbd63245094ad857fc1215aa6a97`  
		Last Modified: Wed, 09 Dec 2020 21:53:32 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
