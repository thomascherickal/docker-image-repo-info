## `adoptopenjdk:15-hotspot-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:f66a1c8030d0c1a24af5ef0119b4644dda95613d9e7520184a61b86bf9b5f790
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `adoptopenjdk:15-hotspot-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

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
