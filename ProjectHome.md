# Delphi-OpenCV #

OpenCV version - 2.4.9<br>
Development environment - Delphi 2010-XE7<br>
<br>
Requires installed <a href='http://www.microsoft.com/ru-ru/download/details.aspx?id=40784'>Visual C++ redistributable for Visual Studio 2013</a>

<h3>Contributors:</h3>
<pre><code> Laentir Valetov (email: laex@bk.ru)
 Mikhail Grigorev (email: sleuthhound@gmail.com)
</code></pre>
<h2>How to install:</h2>
Download the <a href='https://github.com/Laex/Delphi-OpenCV/archive/master.zip'>archive</a>
Unzip it to a convenient directory, thus get the following directory structure<br>
<pre><code>PROJECT_ROOT&gt; - Directory, such as "C:\OpenCV\"
	&lt;bin&gt;
	&lt;redist&gt;
	&lt;resource&gt;
	&lt;samples&gt;
	&lt;source&gt;
</code></pre>
Add the search path for the modules of the project in Delphi IDE (Tools-Options-Delphi Options-Library-Library path)<br>
<pre><code>&lt;PROJECT_ROOT&gt;\source
&lt;PROJECT_ROOT&gt;\source\utils
&lt;PROJECT_ROOT&gt;\source\component
&lt;PROJECT_ROOT&gt;\source\sdl
&lt;PROJECT_ROOT&gt;\source\opengl
&lt;PROJECT_ROOT&gt;\source\ffmpeg
&lt;PROJECT_ROOT&gt;\resource\facedetectxml
</code></pre>
where <code>&lt;PROJECT_ROOT&gt;</code> directory, which was unzipped project.<br>
Add to your PATH variable path to the library "opencv<b><b>.dll" and FFMPEG dll.<br></b> for Win32 <code>&lt;PROJECT_ROOT&gt;\bin\Win32</code>
<i>for Win64 <code>&lt;PROJECT_ROOT&gt;\bin\Win64</code></i>

Or</b>

For 64-bit<br>
<pre><code>1. Copy the dll files from the &lt;PROJECT_ROOT&gt;\redist\VC2013x64\ to C:\Windows\System32\
2. Copy all the dll from &lt;PROJECT_ROOT&gt;\bin\Win64 in the C:\Windows\System32\
3. Copy the dll files from the &lt;PROJECT_ROOT&gt;\redist\VC2013x86\ to C:\Windows\SysWOW64\
4. Copy all the dll from &lt;PROJECT_ROOT&gt;\bin\Win32 in the C:\Windows\SysWOW64\
</code></pre>
For 32-bit<br>
<pre><code>1. Copy the dll files from the &lt;PROJECT_ROOT&gt;\redist\VC2013x86\ to C:\Windows\System32\
2. Copy all the dll from &lt;PROJECT_ROOT&gt;\bin\Win32 in the C:\Windows\System32\
</code></pre>
To install the components, open and install<br>
<pre><code>&lt;PROJECT_ROOT&gt;\source\component\DelphiXX\OpenCVXXX.dpk
&lt;PROJECT_ROOT&gt;\source\component\DelphiXX\dclCommonOpenCVXXX.dpk
&lt;PROJECT_ROOT&gt;\source\component\DelphiXX\dclVCLOpenCVXXX.dpk
&lt;PROJECT_ROOT&gt;\source\component\DelphiXX\dclFMXOpenCVXXX.dpk
</code></pre>
Open in Delphi IDE and compile:<br>
Examples of the use of certain functions and procedures<br>
<pre><code>&lt;PROJECT_ROOT&gt;\samples\LibDemo\LibDemo.groupproj
</code></pre>
Examples of the use of video processing algorithms<br>
<pre><code>&lt;PROJECT_ROOT&gt;\samples\MultiDemo\MultiDemo.groupproj
</code></pre>
Examples of the use of video processing algorithms using VCL.Forms<br>
<pre><code>&lt;PROJECT_ROOT&gt;\samples\VCLDemo\VCLDemo.groupproj
</code></pre>
Examples of using FFMPEG library header files are in the<br>
<pre><code>&lt;PROJECT_ROOT&gt;\samples\FFMpeg\FFMPEG.groupproj
</code></pre>
Examples of use of components<br>
<pre><code>&lt;PROJECT_ROOT&gt;\samples\Components\ComponentsDemo.groupproj
</code></pre>