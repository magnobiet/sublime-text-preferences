# [php.fmt](https://github.com/dericofilho/php.tools) support for Sublime Text 2/3


php.fmt, php.tools and php.oracle aim to help PHP development.

**The following features are available through command palette (`ctrl+shift+P` or `cmd+shift+P`) :**

%CMD%


### Currently Supported Transformations:

%PASSES%

### What does it do?

<table>
<tr>
<td>Before</td>
<td>After</td>
</tr>
<tr>
<td>
<pre><code>&lt;?php
for($i = 0; $i &lt; 10; $i++)
{
if($i%2==0)
echo "Flipflop";
}
</code></pre>
</td>
<td>
<pre><code>&lt;?php
for ($i = 0; $i &lt; 10; $i++) {
	if ($i%2 == 0) {
		echo "Flipflop";
	}
}
</code></pre>
</td>
</tr>
<tr>
<td>
<pre><code>&lt;?php
$a = 10;
$otherVar = 20;
$third = 30;
</code></pre>
</td>
<td>
<pre><code>&lt;?php
$a        = 10;
$otherVar = 20;
$third    = 30;
</code></pre>
<i>This can be enabled with the option "enable_auto_align"</i>
</td>
</tr>
<tr>
<td>
<pre><code>&lt;?php
namespace NS\Something;
use \OtherNS\C;
use \OtherNS\B;
use \OtherNS\A;
use \OtherNS\D;

$a = new A();
$b = new C();
$d = new D();
</code></pre>
</td>
<td>
<pre><code>&lt;?php
namespace NS\Something;

use \OtherNS\A;
use \OtherNS\C;
use \OtherNS\D;

$a = new A();
$b = new C();
$d = new D();
</code></pre>
<i>note how it sorts the use clauses, and removes unused ones</i>
</td>
</tr>
</table>

### What does it do? - PSR version

<table>
<tr>
<td>Before</td>
<td>After</td>
</tr>
<tr>
<td>
<pre><code>&lt;?php
for($i = 0; $i &lt; 10; $i++)
{
if($i%2==0)
echo "Flipflop";
}
</code></pre>
</td>
<td>
<pre><code>&lt;?php
for ($i = 0; $i &lt; 10; $i++) {
    if ($i%2 == 0) {
        echo "Flipflop";
    }
}
</code></pre>
<i>Note the identation of 4 spaces.</i>
</td>
</tr>
<tr>
<td>
<pre><code>&lt;?php
class A {
function a(){
return 10;
}
}
</code></pre>
</td>
<td>
<pre><code>&lt;?php
class A
{
    public function a()
    {
        return 10;
    }
}
</code></pre>
<i>Note the braces position, and the visibility adjustment in the method a().</i>
</td>
</tr>
<tr>
<td>
<pre><code>&lt;?php
namespace NS\Something;
use \OtherNS\C;
use \OtherNS\B;
use \OtherNS\A;
use \OtherNS\D;

$a = new A();
$b = new C();
$d = new D();
</code></pre>
</td>
<td>
<pre><code>&lt;?php
namespace NS\Something;

use \OtherNS\A;
use \OtherNS\C;
use \OtherNS\D;

$a = new A();
$b = new C();
$d = new D();
</code></pre>
<i>note how it sorts the use clauses, and removes unused ones</i>
</td>
</tr>
</table>

### Installation

#### Requirements
- **You must have a running copy of PHP on the machine you are running Sublime Text**

Plugin runs with PHP 5.6 or newer installed in the machine running the plugin.

There is a backwards compatible mode with PHP 5.5 - however not all improvements will be available in this mode.

#### Install this plugin through Package Manager.

- In Sublime Text press `ctrl+shift+P`
- Choose `Package Control: Install Package`
- Choose `phpfmt`

#### Configuration (Windows)

- Edit configuration file located at `%AppData%\Sublime Text 2\Packages\phpfmt\phpfmt.sublime-settings`
- For field `"php_bin"` enter the path to the php.exe
  Example: `"php_bin":"c:/PHP/php.exe"`

### Settings

Prefer using the toggle options at command palette. However you might find yourself in need to setup where PHP is running, use this option below for the configuration file.
```
{
"php_bin":"/usr/local/bin/php",
}
```

### Troubleshooting
- Be sure you can run PHP from the command line.
- If you are a MAMP user, please use the MAMP's PHP binary to execute the plugin. This issue might be handy to help you configure the plugin: https://github.com/dericofilho/sublime-phpfmt/issues/109

### Acknowledgements
- GoSublime - for the method to update the formatted buffer
- Google's diff match patch - http://code.google.com/p/google-diff-match-patch/
