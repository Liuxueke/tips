消息提示调用方法：

<div class="fmt" id="wmd-preview"><pre class="hljs javascript" style="background-color: transparent;"><span class="diff"><code><span class="hljs-function"><span class="hljs-keyword">function</span> <span class="hljs-title">infor_tck</span><span class="hljs-params">(ifo)</span></span>{
    <span class="hljs-keyword">if</span>($(<span class="hljs-string">".dialog_infor"</span>).hasClass(<span class="hljs-string">'alreadyClick'</span>)){
        <span class="hljs-keyword">return</span> <span class="hljs-literal">false</span>;
    }
    $(<span class="hljs-string">'body'</span>).append(<span class="hljs-string">'&lt;div class="dialog_infor alreadyClick fs14"&gt;'</span>+ifo+<span class="hljs-string">'&lt;/div&gt;'</span>);
    setTimeout(<span class="hljs-function"><span class="hljs-keyword">function</span><span class="hljs-params">()</span></span>{
        $(<span class="hljs-string">'.dialog_infor'</span>).fadeOut().remove();
    },<span class="hljs-number">2000</span>);
}</code></span></pre></div>

infor_tck('您输入的密码不正确！');



