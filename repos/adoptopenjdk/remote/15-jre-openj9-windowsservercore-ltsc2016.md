## `adoptopenjdk:15-jre-openj9-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:3543a90a9a22b97117fd747621105af76ef7622d32e8db83674a252dc5970648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `adoptopenjdk:15-jre-openj9-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull adoptopenjdk@sha256:a52b6f8a345fb33723b49f3c45ce1a64edb0fe860a81aeab656ab53f07610cfb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5863877139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0179f494718b91e7f44b0413726634eee67364d24a01a75aff67fe28ccc7dfb4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 21:34:58 GMT
ENV JAVA_VERSION=jdk-15.0.1+9_openj9-0.23.0
# Wed, 09 Dec 2020 21:41:45 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9_openj9-0.23.0/OpenJDK15U-jre_x64_windows_openj9_15.0.1_9_openj9-0.23.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9_openj9-0.23.0/OpenJDK15U-jre_x64_windows_openj9_15.0.1_9_openj9-0.23.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (921c4f8ec53b91b77f6f30ba182474cf53eb937e2edc944ba9f3f6a4262450ea) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '921c4f8ec53b91b77f6f30ba182474cf53eb937e2edc944ba9f3f6a4262450ea') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 21:41:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
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
	-	`sha256:7936991db76fe16143811b69d35d076062f0c0f45e89d8afad60c9b2299a5380`  
		Last Modified: Wed, 09 Dec 2020 22:35:56 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98aacc58265282fcbc994b24818e33788aa1178b53daa6cf865cbdd7e9b3132`  
		Last Modified: Wed, 09 Dec 2020 22:37:25 GMT  
		Size: 95.0 MB (95029729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3898a0745eb9cf1e686607693275ad5ec385549fea0579a2320f92627ebec635`  
		Last Modified: Wed, 09 Dec 2020 22:37:12 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
