## `python:rc-windowsservercore-ltsc2022`

```console
$ docker pull python@sha256:51f1f823a6922cf4d2682e9fbb531ef6897d423dbec259e4d151ecfeb6901fc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.169; amd64

### `python:rc-windowsservercore-ltsc2022` - windows version 10.0.20348.169; amd64

```console
$ docker pull python@sha256:096a1a0d075dc2584041b5b3699c525e81c9d4b8dbde64dfa19881b3288dc0a4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2307075367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4819ef81237b1ecee59a3417b2e1eb0d5f7d33442e362ba26a9b0d485a374140`
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
# Wed, 08 Sep 2021 00:15:11 GMT
ENV PYTHON_VERSION=3.10.0rc2
# Wed, 08 Sep 2021 00:15:12 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 08 Sep 2021 00:16:45 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 08 Sep 2021 00:16:47 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 08 Sep 2021 00:16:48 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 08 Sep 2021 00:16:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 08 Sep 2021 00:16:50 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 08 Sep 2021 00:17:48 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 08 Sep 2021 00:17:49 GMT
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
	-	`sha256:d75b03a5e4b1c874b59bc806c6ebb7a6bd776a1b9df1c9feedddc00e2f8844d0`  
		Last Modified: Wed, 08 Sep 2021 00:30:32 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a04e6d36439a5483c5ff2e433586e941aaffad96d69faa828457bac45e3e50`  
		Last Modified: Wed, 08 Sep 2021 00:30:32 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740c627d5ff64f08c8dc76b42d3574df0e8bdb5e1bba6def208077e638d28b53`  
		Last Modified: Wed, 08 Sep 2021 00:30:38 GMT  
		Size: 47.3 MB (47276040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ab67f449fb240df721afe7954b6e272420a230011465e0fdbc8528bce0cffd`  
		Last Modified: Wed, 08 Sep 2021 00:30:32 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6475c3c38eb7928b0236a359df04145586a2826ab905b29a01f65460dd8e58`  
		Last Modified: Wed, 08 Sep 2021 00:30:29 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bfa7e2be69048bd039aa5de8c9f54c1c144acb52b0c943e5a1d5492acea5a9`  
		Last Modified: Wed, 08 Sep 2021 00:30:29 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21887883e060dd8b15f7f518e0652f8e01ba01286c320247d0061728587ee3e8`  
		Last Modified: Wed, 08 Sep 2021 00:30:29 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9dce3898a7e5f64137a6eb597b6deb6cf3b8b309192fc5b5ab2bc17dd75969`  
		Last Modified: Wed, 08 Sep 2021 00:30:31 GMT  
		Size: 6.7 MB (6698455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69d544741669a1d172d40f1cf3b5834c50b431a4f93d49ea1c8f4ce80414ddf`  
		Last Modified: Wed, 08 Sep 2021 00:30:29 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
