## `python:rc-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:9dd976c8e8f688f8cec65fa904e16ec621226578f412671e8ae2b1a297b7e6ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `python:rc-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull python@sha256:c45494b691542d67adacd14af605463cabe5cdbed0386ca81ff121083ac5f7be
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6324385101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49f22bbf150315623ef1bd7278dcb97c58ab65bce1d8539e0a5c5b9b53129f56`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:16:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 16:15:59 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 08 Sep 2021 00:21:47 GMT
ENV PYTHON_VERSION=3.10.0rc2
# Wed, 08 Sep 2021 00:21:48 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 08 Sep 2021 00:23:40 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 08 Sep 2021 00:23:41 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 08 Sep 2021 00:23:42 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 08 Sep 2021 00:23:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 08 Sep 2021 00:23:44 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 08 Sep 2021 00:25:07 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 08 Sep 2021 00:25:08 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f888b02e4880b5280aedf776d35ce62a07f97c9f4671b4e167d0fadfbcd663f`  
		Last Modified: Wed, 25 Aug 2021 13:39:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed309cb6c9da38c0fcf25249903316fc3e48f586b18fda16f3ed427ce99793d`  
		Last Modified: Wed, 25 Aug 2021 16:27:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9425a37e5aa07b8652e5dfecdf6b0038bc1d9febb1135df2f29e68c9b9504708`  
		Last Modified: Wed, 08 Sep 2021 00:31:15 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd51abf1813673c8322fbbe1985b83fb1aa498fbdea69258b3162f162307080`  
		Last Modified: Wed, 08 Sep 2021 00:31:15 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210e6d587f6405554314dac68a5195941cd09ba94dd0508a8d3be5bdffc9c786`  
		Last Modified: Wed, 08 Sep 2021 00:32:07 GMT  
		Size: 47.0 MB (46961813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae71e35c1bf4a9a7aefe8f0e9b64462c0e2f6396d05f7d6332aef081ad9194e3`  
		Last Modified: Wed, 08 Sep 2021 00:31:15 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b23db0b382925b318d7e615793bd3b23d19fd651f88c154864ce73890122908`  
		Last Modified: Wed, 08 Sep 2021 00:31:13 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7c1f486d458fd4aaa091f57bed62f5fd4489afae7d28c31d6de87586933307`  
		Last Modified: Wed, 08 Sep 2021 00:31:13 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eca6a1aad6e13700255296c2eac6381487c707ef70c5ca19f6c1654a97fcd4b`  
		Last Modified: Wed, 08 Sep 2021 00:31:13 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef42df51f34d515147270771aa32a809a8290f13d3907133a87eeaee1526175`  
		Last Modified: Wed, 08 Sep 2021 00:31:15 GMT  
		Size: 6.4 MB (6444611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52237695d5e8efd96d776d8efd944840597e0afab4cdba08985f7f76de5f8d1`  
		Last Modified: Wed, 08 Sep 2021 00:31:13 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
