## `adoptopenjdk:13-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:adc88c6f9ee90b4d3b1daa8b1f89de3a5e73b9083e594308dd0ea9306f089b36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `adoptopenjdk:13-hotspot-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

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
