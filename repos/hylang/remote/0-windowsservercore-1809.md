## `hylang:0-windowsservercore-1809`

```console
$ docker pull hylang@sha256:aa324c28083b7206a13775db4f06300cb86cccc7280b0958b57b6ff2297fe847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `hylang:0-windowsservercore-1809` - windows version 10.0.17763.1697; amd64

```console
$ docker pull hylang@sha256:71a75c0714a8f57104388bdb1da6e454a80b322b8f0d2c340a76c5588a579ff7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2509880193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4559fa6ec8cfe806b699edd883b7c164db2c90841c91f9c91c097062fb408cf`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 08 Jan 2021 08:50:52 GMT
RUN Install update 1809-amd64
# Wed, 13 Jan 2021 13:13:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 19:12:32 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 13 Jan 2021 19:26:36 GMT
ENV PYTHON_VERSION=3.8.7
# Wed, 13 Jan 2021 19:26:36 GMT
ENV PYTHON_RELEASE=3.8.7
# Wed, 13 Jan 2021 19:28:12 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 19:28:13 GMT
ENV PYTHON_PIP_VERSION=20.3.3
# Wed, 13 Jan 2021 19:28:14 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5f38681f7f5872e4032860b54e9cc11cf0374932/get-pip.py
# Wed, 13 Jan 2021 19:28:15 GMT
ENV PYTHON_GET_PIP_SHA256=6a0b13826862f33c13b614a921d36253bfa1ae779c5fbf569876f3585057e9d2
# Wed, 13 Jan 2021 19:28:58 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 13 Jan 2021 19:28:59 GMT
CMD ["python"]
# Thu, 14 Jan 2021 01:18:02 GMT
ENV HY_VERSION=0.19.0
# Thu, 14 Jan 2021 01:18:41 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Thu, 14 Jan 2021 01:18:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4dcc9a9b9e680514ef3fdfcc2ce08a3768f9e412703faa137f4a7c8297600052`  
		Size: 717.4 MB (717439216 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e00081a98bb2679c3c5f469e09d475980133a20987f9cae4cf4f7aedf59f9d8f`  
		Last Modified: Wed, 13 Jan 2021 13:17:19 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f229e126d7cfc5407c75c0703062a138f0024cbcf6a1b318a0c87ba901af90a5`  
		Last Modified: Wed, 13 Jan 2021 19:41:55 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149436224fab0a1df709fd99c825b8e199abc84f739d09457dc5de68bdd0e4c5`  
		Last Modified: Wed, 13 Jan 2021 19:44:10 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a6839d9d2d5211582624c51fccdaf52913b66c1d69a592867f6e470dc8e480`  
		Last Modified: Wed, 13 Jan 2021 19:44:10 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f002852607392544cc038a6423b50988db3e500ed4c372f81bf308461b29b777`  
		Last Modified: Wed, 13 Jan 2021 19:45:21 GMT  
		Size: 58.3 MB (58282287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc0c73ef7826b7a6e86333b192e1da4c0d802047b06a63039ad6bfeaa74fb74`  
		Last Modified: Wed, 13 Jan 2021 19:44:07 GMT  
		Size: 1.1 KB (1087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676bb0ccd357edeb9d9c2d0105645271fa6af219b81371c634c087b4593a7635`  
		Last Modified: Wed, 13 Jan 2021 19:44:06 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4304cf5a2de52538dd5ab3741718e84abf5588d7a8e4dc39652747f50a70ed11`  
		Last Modified: Wed, 13 Jan 2021 19:44:06 GMT  
		Size: 1.1 KB (1087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d93febb8333a795f0677ee58ce2fd09908273a680c2a9ec0a4e53eb2d8d096`  
		Last Modified: Wed, 13 Jan 2021 19:44:10 GMT  
		Size: 10.3 MB (10296765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78f46610c9a8c218ed44a911e09c43edca5632680c953a351d61aaf49606da3`  
		Last Modified: Wed, 13 Jan 2021 19:44:05 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92552deabf0a7e46eaf03f9860efabe8229d69e7b6c0483741d13a02b192f24b`  
		Last Modified: Thu, 14 Jan 2021 01:24:44 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18f925473d6d0a67af2b37b47d347a213c5438a297a54626badd86321e918f7`  
		Last Modified: Thu, 14 Jan 2021 01:24:48 GMT  
		Size: 5.5 MB (5517885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c89d2d9963152d6d4709c79e30fc3a7a43dd9c37ae3993ed2ecee5b94582ac2`  
		Last Modified: Thu, 14 Jan 2021 01:24:44 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
