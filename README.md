<h3>Usage Example</h3>
<pre class="lang-php prettyprint prettyprinted" style=""><code><span class="pln">$message </span><span class="pun">=</span><span class="pln"> </span><span class="str">'Ready your ammunition; we attack at dawn.'</span><span class="pun">;</span><span class="pln">
$key </span><span class="pun">=</span><span class="pln"> hex2bin</span><span class="pun">(</span><span class="str">'000102030405060708090a0b0c0d0e0f101112131415161718191a1b1c1d1e1f'</span><span class="pun">);</span><span class="pln">

$encrypted </span><span class="pun">=</span><span class="pln"> </span><span class="typ">SaferCrypto</span><span class="pun">::</span><span class="pln">encrypt</span><span class="pun">(</span><span class="pln">$message</span><span class="pun">,</span><span class="pln"> $key</span><span class="pun">);</span><span class="pln">
$decrypted </span><span class="pun">=</span><span class="pln"> </span><span class="typ">SaferCrypto</span><span class="pun">::</span><span class="pln">decrypt</span><span class="pun">(</span><span class="pln">$encrypted</span><span class="pun">,</span><span class="pln"> $key</span><span class="pun">);</span><span class="pln">

var_dump</span><span class="pun">(</span><span class="pln">$encrypted</span><span class="pun">,</span><span class="pln"> $decrypted</span><span class="pun">);</span></code></pre>
