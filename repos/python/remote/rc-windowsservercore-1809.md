## `python:rc-windowsservercore-1809`

```console
$ docker pull python@sha256:a3f87743ce000c6a0f40d9e99e473eb240fe4f7c7d4ad9cc7e90ab6ce2e14e0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `python:rc-windowsservercore-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull python@sha256:877ad52d1ed4dcb0f2c80a701666f48db0b8a684def895e2af72bceb54ed8c97
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2456781960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc65cc1348aaa401290a819838d11155677a48ea5761349ac0ac430a6003571`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 03 Nov 2020 03:11:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Nov 2020 13:26:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Nov 2020 17:13:40 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 11 Nov 2020 17:13:40 GMT
ENV PYTHON_VERSION=3.10.0a2
# Wed, 11 Nov 2020 17:13:41 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 11 Nov 2020 17:15:20 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 02 Dec 2020 00:16:59 GMT
ENV PYTHON_PIP_VERSION=20.3
# Wed, 02 Dec 2020 00:16:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2357a5f805565496648ebf597bcffe9e2d9ce379/get-pip.py
# Wed, 02 Dec 2020 00:17:00 GMT
ENV PYTHON_GET_PIP_SHA256=7f28b41ce236af61a00dfcbd6fd38c52d46488ece91fb4585b95775b076bbc85
# Wed, 02 Dec 2020 01:18:07 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 02 Dec 2020 01:18:09 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:680bbdbacf1bcbace70de5087d02d31e9dd7a22feae59f746f54dab46c1d5bda`  
		Size: 669.7 MB (669696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da5a67a9f3a363cb69c8104913a5a58c1c47e8f648a07d057fc28a5f98790e60`  
		Last Modified: Wed, 11 Nov 2020 13:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba27fafdef0dd2d90225160fe1fa0393acbcfbe112b6442bf74fa7f41916bcfb`  
		Last Modified: Wed, 11 Nov 2020 17:38:15 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d151bd581671d37a546f79c9c5afda96cd407e11d445b3e1b7a4cbcc25146c`  
		Last Modified: Wed, 11 Nov 2020 17:38:14 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18844c027dd533aa266555588e3065a0ac21230d148ad96e069d44e59d75b77a`  
		Last Modified: Wed, 11 Nov 2020 17:38:14 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e474d026f79d1340dd26f1d903adcbb315af64d8c8571289e5c49884ca916ee1`  
		Last Modified: Wed, 11 Nov 2020 17:38:22 GMT  
		Size: 58.4 MB (58383816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ddd5c1423c30938971858e2f80bdb39b3b734b3abad42738ee78ffc8b57964`  
		Last Modified: Wed, 02 Dec 2020 01:28:05 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3db10ff66de59130498e7001e76670f5987e67bc14103b9d877b9b3a7cda1af`  
		Last Modified: Wed, 02 Dec 2020 01:28:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d4bb43851e0c3c732cd5e67da318d9532b1a1dffa2154ed644c471395c326a`  
		Last Modified: Wed, 02 Dec 2020 01:28:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c03440eb585d4cb79bd259cb40853ad7b82b6efafbc1acb1a4a5bc0fc5a3cd`  
		Last Modified: Wed, 02 Dec 2020 01:28:08 GMT  
		Size: 10.4 MB (10359731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a0228e2ffb26f09dadfcde23c5aaae32f639a29f8bf99250ef80bca3d4e9bd`  
		Last Modified: Wed, 02 Dec 2020 01:28:04 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
