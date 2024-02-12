# wheel 

.whl file for Python, also known as a wheel file, is a built distribution of a Python package. It’s essentially a ZIP archive with a specially crafted filename that tells installers what Python versions and platforms the wheel will support.

This repository informs users how to create a .whl file on Windows operating system automatically.

<pre>
On Windows, vs_BuildTools.exe should be downloaded from Microsoft.
https://aka.ms/vs/17/release/vs_buildtools.exe
Run the follwing command to install vs_BuildTools which automatically downloads the necessary tools.

$ ./vs_BuildTools.exe --norestart --passive --downloadThenInstall --includeRecommended --add Microsoft.VisualStudio.Workload.NativeDesktop --add Microsoft.VisualStudio.Workload.VCTools --add Microsoft.VisualStudio.Workload.MSBuildTools

Download git clone for creating application wheel.
For example, 
$ git clone https://github.com/hamiltron/py-simple-audio.git
$ cd py-simple-audio
Run the following command to generate wheel.
$ python setup.py bdist_wheel
*** is the target wheel file in dist directory.
$ pip install dist/***.whl

</pre>
