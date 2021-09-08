## `python:3-windowsservercore`

```console
$ docker pull python@sha256:472c3baca18f0a89c9c945460b05f621402ea624f593270e6509ec861cba6f97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.169; amd64
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `python:3-windowsservercore` - windows version 10.0.20348.169; amd64

```console
$ docker pull python@sha256:5b65a4b4fac557af914b6e65285b09232ec6c12cca4d8624d64383477e6c7343
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2309863471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14533a6ed7b5b0b7085f432e82933798259139c0a6b34eece2f584e501be5166`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Mon, 09 Aug 2021 15:38:40 GMT
RUN Install update ltsc2022-amd64
# Fri, 27 Aug 2021 17:23:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 03 Sep 2021 01:15:07 GMT
ENV PYTHONIOENCODING=UTF-8
# Fri, 03 Sep 2021 01:17:41 GMT
ENV PYTHON_VERSION=3.9.7
# Fri, 03 Sep 2021 01:17:42 GMT
ENV PYTHON_RELEASE=3.9.7
# Fri, 03 Sep 2021 01:18:52 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Fri, 03 Sep 2021 01:18:53 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 08 Sep 2021 00:25:28 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 08 Sep 2021 00:25:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 08 Sep 2021 00:25:30 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 08 Sep 2021 00:26:20 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 08 Sep 2021 00:26:22 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:393f6f5bddce764d78d9d19db836750d03ca4866c2ec9b794853a461e6f2cf63`  
		Size: 1.0 GB (1001389105 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:788c1927703ffa41d5a2f1824a9c9f2d663fdc9e50b2b49387de1cb0c1b33aa4`  
		Last Modified: Fri, 27 Aug 2021 17:40:17 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b9151efee2499c1021ea6e74f4805e04d77cb2f3931220e40b7a1c5012d7bd`  
		Last Modified: Fri, 03 Sep 2021 01:20:56 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e724eb872c9e66c85dd24c6be08931bf32188a7acf65061e6353a271175c9d88`  
		Last Modified: Fri, 03 Sep 2021 01:21:18 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df741e44b999185d1e13b88d0217c76c1e5773efb3d18ed96f8064b15de76e83`  
		Last Modified: Fri, 03 Sep 2021 01:21:17 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5190d67d952a8ecc944123570a4a81c3a6ec408908af3b822710389015458a35`  
		Last Modified: Fri, 03 Sep 2021 01:21:28 GMT  
		Size: 50.2 MB (50230759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4568f1c9eaa663d34a0051efe056a357c84d4f3fe950014e557e359bbe7805b`  
		Last Modified: Fri, 03 Sep 2021 01:21:15 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380dd44be77d68306b5b2d71d5d43d61292a6d041a431367e1a0023b740c80fd`  
		Last Modified: Wed, 08 Sep 2021 00:32:20 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d466e5f42c6ecd7b4390a9ed3ad4ba557f49975454917356dc25d00dd5980b`  
		Last Modified: Wed, 08 Sep 2021 00:32:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40cc8622eb3413cf88b4fdf5efb8e579e70ecc9addb5e60402e680a03ff58fa`  
		Last Modified: Wed, 08 Sep 2021 00:32:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da94e78b1b371cd37b4c7dc1d512460e36084f8a1ec0d35e59f9a15ce68717fa`  
		Last Modified: Wed, 08 Sep 2021 00:32:27 GMT  
		Size: 6.5 MB (6531883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47206816647ca533218d9be088e96e80984af8743f1238d9a1547e58c5feba9a`  
		Last Modified: Wed, 08 Sep 2021 00:32:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull python@sha256:847c24877dbd26d4128b0ac3d5ab66213476c991e4844597028648c90a400697
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742342712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf63c978a30d4b8787f4d6124a18c82beb1153c2f198e41b6672d99ec1bc6e4a`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 12:35:53 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 31 Aug 2021 18:15:17 GMT
ENV PYTHON_VERSION=3.9.7
# Tue, 31 Aug 2021 18:15:18 GMT
ENV PYTHON_RELEASE=3.9.7
# Tue, 31 Aug 2021 18:17:04 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 31 Aug 2021 18:17:05 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 08 Sep 2021 00:26:29 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 08 Sep 2021 00:26:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 08 Sep 2021 00:26:32 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 08 Sep 2021 00:27:55 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 08 Sep 2021 00:27:58 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723798581711620321543fadca5f5b861c2af4dafbe2c3acdb59945488cf07f9`  
		Last Modified: Wed, 25 Aug 2021 12:42:48 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b684a127bb8c10cc6f53031849b1087be1beb93e1747099a52b945110c4d95a`  
		Last Modified: Tue, 31 Aug 2021 18:22:20 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e0c0c3e9a11e4a195182a593e149c539e17651a37871060e3917a41bcf734c`  
		Last Modified: Tue, 31 Aug 2021 18:22:20 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d5745da387ba09f57d52ebe4cb48eb1c09d61362d0394ab22c766c046a7ab1`  
		Last Modified: Tue, 31 Aug 2021 18:23:13 GMT  
		Size: 50.0 MB (50015961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18492fa4e1c8990c50de0f5e3596d9510792058379866818ce1373a52fc32378`  
		Last Modified: Tue, 31 Aug 2021 18:22:17 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8855122529cb80d0cb1b4b72a85cb3bc631e52d693f2b2a188a8b6207d5c11c3`  
		Last Modified: Wed, 08 Sep 2021 00:32:43 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac8abc9be3bb358886d47c932c54e584a2533afebdac109dc3380b3562538ab`  
		Last Modified: Wed, 08 Sep 2021 00:32:43 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb7fa98469cbf79b5a02be9bcdc015c18ded6f2fd5007145b4f8f5db51ac2ac`  
		Last Modified: Wed, 08 Sep 2021 00:32:44 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3758726bba8f150c018946ee18d3ae67157e82dd4578e6a9ff55b2580c7f1d`  
		Last Modified: Wed, 08 Sep 2021 00:32:50 GMT  
		Size: 6.3 MB (6316414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc89d6e62dde34485724452fcf09532cafd778249cb037de4ea4fd8aaa54288`  
		Last Modified: Wed, 08 Sep 2021 00:32:43 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull python@sha256:39a46c1ada84fc76c4888357d641b35ce482cc820fc2728ed13eab67ebe7b7c5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6327173456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53153b72eca2345af66e02a1e38c4cf72c3c5d5513410e2565cc82df5b58bad9`
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
# Tue, 31 Aug 2021 18:18:28 GMT
ENV PYTHON_VERSION=3.9.7
# Tue, 31 Aug 2021 18:18:29 GMT
ENV PYTHON_RELEASE=3.9.7
# Tue, 31 Aug 2021 18:20:08 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 31 Aug 2021 18:20:09 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 08 Sep 2021 00:28:09 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 08 Sep 2021 00:28:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 08 Sep 2021 00:28:11 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 08 Sep 2021 00:29:34 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 08 Sep 2021 00:29:36 GMT
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
	-	`sha256:039fa6cb83e9802bcdf801b9970ecd556db205120821e0414b09e00befd4c4d2`  
		Last Modified: Tue, 31 Aug 2021 18:23:30 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbea45e4d3ff243223e1823f36a2db84414c073036662c3c6c122f2041eaf04`  
		Last Modified: Tue, 31 Aug 2021 18:23:30 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c9cd21e3c832e7deb1095109fd74fbc31758d8c5f604258eb786e72d971074`  
		Last Modified: Tue, 31 Aug 2021 18:23:37 GMT  
		Size: 49.9 MB (49918725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017004522cdf8e220819135b9032282a5a026becbc4344d69f8f05704388b902`  
		Last Modified: Tue, 31 Aug 2021 18:23:27 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0919781bc5c9b371211e152cbb5049229c42a081dd26740094c35fad7776e7a2`  
		Last Modified: Wed, 08 Sep 2021 00:33:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01863e95a44482104745a9235ad16e011d404b4800061ce703ba56658fd69b1e`  
		Last Modified: Wed, 08 Sep 2021 00:33:06 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0808e7873a874c46130b4be3511b5b00254769bbb6086d67d7032a852d96273`  
		Last Modified: Wed, 08 Sep 2021 00:33:06 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714efc9b4e4b974b155449610eb1e07a1ed977af9686391358d848b2b960b595`  
		Last Modified: Wed, 08 Sep 2021 00:33:08 GMT  
		Size: 6.3 MB (6276125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf94347f2551df785180affc557f54a92f923bad52bfe7e961cf606f2cb27a8`  
		Last Modified: Wed, 08 Sep 2021 00:33:06 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
