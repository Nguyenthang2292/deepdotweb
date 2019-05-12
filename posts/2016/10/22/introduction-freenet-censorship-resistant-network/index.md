---
Introduction to Freenet: A Censorship-Resistant Network
---
<article class="post-listing post-15981 post type-post status-publish format-standard has-post-thumbnail hentry category-articles category-deepdot-news tag-censorshipresistant tag-freenet tag-introduction tag-network">
    <div class="post-inner">
    <p class="post-meta">
    <span>Posted by: <a href="https://www.deepdotweb.com/author/ciphas/" title="">Ciphas </a></span>
    <span>October 22, 2016</span>
    <span>in <a href="https://www.deepdotweb.com/category/articles/" rel="category tag">Articles</a>, <a href="https://www.deepdotweb.com/category/deepdot-news/" rel="category tag">Featured</a></span>
    <span><a href="https://www.deepdotweb.com/2016/10/22/introduction-freenet-censorship-resistant-network/#comments">7 Comments</a></span>
    </p>
    <div class="clear"></div>
    <div class="entry">
    <p>I don’t know about you, but I’m not a fan of censorship; I would think that most privacy-minded Tor users would agree.</p>
    <p>If you’re part of this crowd, have you used Freenet yet? Though it functions quite a bit differently than Tor and I2P, it still has its advantages in terms of pseudonymity.</p>
    <p><strong>A Brief Explanation</strong></p>
    <p><strong><img class="wp-image-15982 aligncenter" src="https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-13.jpeg" srcset="https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-13.jpeg 638w, https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-13-300x225.jpeg 300w" sizes="(max-width: 638px) 100vw, 638px" /></strong></p>
    <p>Credit: freesocial.draketo.de</p>
    <p>Freenet enables the user (that would be you) to create a fake computer-generated identity so that others won’t know who you are – unless you choose to share that information.</p>
    <p>It does this through a system called the Web of Trust (WoT), which helps filter out spam, bots, and other unwelcome identities. The WoT consists of a network of pseudonymous identities generated by the network when you first join.</p>
    <p>If you were to create a new identity, it might look something like this: “ap_subgratis.” While you can generate another identity if you don’t like the first one, the developers don’t recommend this, as it could, in theory, break your anonymity.</p>
    <p>The WoT consists of these objects:</p>
    <ul>
    <li><strong>Identities </strong>are those using the system</li>
    <li><strong>Own identities </strong>are identities which belong to you</li>
    <li><strong>Trust values</strong> are ratings between pairs of identities. They range from -100 to +100, and any identity in the network can assign a rating to any other.</li>
    <li><strong>Score values </strong>exist between pairs of identities and non-identities; the plugin computes these values for each identity. Only one rating exists for each pair; if a score is negative, clients should not download content from that identity.</li>
    <li><strong>Puzzles</strong> serve the purpose of introducing new identities to the Web of Trust. Types of puzzles include the familiar captcha, as well as audio captchas.</li>
    </ul>
    <p>The more puzzles you solve, the more you can gain trust within the WoT (as weird as that may sound).</p>
    <p><img class="wp-image-15983 aligncenter" src="https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-66.png" srcset="https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-66.png 1024w, https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-66-300x225.png 300w" sizes="(max-width: 1024px) 100vw, 1024px" /></p>
    <p>Credit: freesocial.draketo.de</p>
    <p><strong>Privacy Features</strong></p>
    <p>If you’re already a Tor user, you might wonder how Freenet is any different. While Tor allows anonymous access to the clearnet, as well as the ability to access its hidden services (a.k.a. onion sites), Freenet is a self-contained network.</p>
    <p>It is <em>not</em> a proxy to the clearnet, i.e. you can’t access sites like Google, Twitter, etc. What Freenet does have are its own websites, filesharing, email, messaging, forums, and chat, all hosted within the network.</p>
    <p>Freenet uses a distributed data store for keeping and delivering information. In other words, information is stored on more than one node. All Freenet nodes contribute a portion of their hard drive space to store pieces of encrypted files.</p>
    <p><img class="wp-image-15984 aligncenter" src="https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image.gif" /></p>
    <p>Now, some may see this as a disadvantage, but on Freenet, you have little control over what type of content is kept in your datastore. Files are kept or deleted based on their popularity, which is one of the ways that Freenet is kept censorship-resistant.</p>
    <p>While it’s not impossible to figure out what encrypted file pieces are kept in your datastore, it would be an arduous process to decrypt them. The point is that if you don’t know what’s being kept in your datastore, it allows plausible deniability.</p>
    <p><strong>Communication Breakdown!</strong></p>
    <p><strong><img class="wp-image-15985 aligncenter" src="https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-14.jpeg" srcset="https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-14.jpeg 638w, https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-14-300x225.jpeg 300w" sizes="(max-width: 638px) 100vw, 638px" /></strong></p>
    <p>Other popular features within Freenet are the Freenet Message System (FMS), and Sone, which is a social network plugin.</p>
    <p>FMS is the most widely used forum system on Freenet. However, it’s not part of the official Freenet codebase, because FMS is written in C++, which is less secure than Java (i.e. the codebase for the rest of Freenet).</p>
    <p>If you’re already on Freenet and are interested in trying out FMS, use this link: <a href="http://localhost:8888/USK@0npnMrqZNKRCRoGojZV93UNHCMN-6UU3rRSAmP6jNLE,~BG-edFtdCC1cSH4O3BWdeIYa8Sw5DfyrSV-TKdO5ec,AQACAAE/fms/142/">FMS Install</a>.</p>
    <p>Sone implements a social network (loosely based on Facebook) on top of Freenet. It requires the Web of Trust in order to connect with other users, so make sure you load that before trying to use Sone. In versions 0.6.5 and beyond, Sone features an FCP interface that allows other applications to access Sone.</p>
    <p><img class="wp-image-15986 aligncenter" src="https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-67.png" srcset="https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-67.png 985w, https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-67-300x169.png 300w" sizes="(max-width: 985px) 100vw, 985px" /></p>
    <p>So imagine a social network, kind of like Facebook, except everyone on it uses fake identities. I kind of like that idea, personally!</p>
    <p>As opposed to Facebook, you won’t have targeted ads showing up constantly (“Got ED? You know you want Cialis!”)</p>
    <p><strong>Freedom of Expression</strong></p>
    <p><strong><img class="wp-image-15987 aligncenter" src="https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-68.png" srcset="https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-68.png 1200w, https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-68-300x142.png 300w, https://www.deepdotweb.com/wp-content/uploads/2016/10/word-image-68-1024x484.png 1024w" sizes="(max-width: 1200px) 100vw, 1200px" /></strong></p>
    <p>Freenet allows you to publish hidden services anonymously as well, known as Freesites. They’re more or less equivalent to Tor’s .onion sites.</p>
    <p>The Freesites are listed in various directories, known as Nerdageddon, Enzo’s Index, and the Censored Index.</p>
    <p>Nerdageddon features this description: “Welcome to Nerdageddon. Here we aim to bring you a list of all freesites, both old and new, which could be interesting to political nerds. The links presented here exclude the sites which Linkageddon flags as porn or cp, and those which I perceive as normal.”</p>
    <p>Linkageddon, for those of you who don’t know, is an uncensored link list that shows every freesite, regardless of its content. As on Tor, you may find CP or gore on Freenet; the difference with Freenet, I feel, is that it gives you sufficient warning about content that you’re about to view. If it doesn’t, you have the option of mentioning it to the community via Sone or FMS.</p>
    <p>Tor, on the other hand, can <em>sometimes</em> feel like the Wild West. There might be shady activity going on all around you, but you’re powerless to stop it!</p>
    <p>Speaking of which, creating your own Freesite is quite simple. You can build it using whatever HTML tool you prefer, and then upload it using jSite, a Freesite uploading tool created by developer Bombe. For more details on creating a Freesite, see <a href="https://wiki.freenetproject.org/JSite">Freenet Wiki: jSite</a>.</p>
    <p><strong>To Join or Not to Join</strong></p>
    <p>Whether or not you decide to try out Freenet is a matter of personal preference. Yes, like Tor, it has its downsides, but in terms of privacy and existing within a small, close-knit online community, it’s one of the best.</p>
    <p>If you’re merely one of the curious types (especially someone who values privacy and anonymity), I’d say take a look. You may like it after all. It’s available at <a href="https://www.freenetproject.org">Freenet Project</a>.</p>
    <p>Besides, where else can you get a name like “am_moraphille”?</p>
    </div>
    <span style="display:none"><a href="https://www.deepdotweb.com/tag/censorshipresistant/" rel="tag">censorshipresistant</a> <a href="https://www.deepdotweb.com/tag/freenet/" rel="tag">freenet</a> <a href="https://www.deepdotweb.com/tag/introduction/" rel="tag">introduction</a> <a href="https://www.deepdotweb.com/tag/network/" rel="tag">network</a></span> <span style="display:none" class="updated">2016-10-22</span>
    <div style="display:none" class="vcard author" itemprop="author" itemscope itemtype="http://schema.org/Person"><strong class="fn" itemprop="name"><a href="https://www.deepdotweb.com/author/ciphas/" title="Posts by Ciphas" rel="author">Ciphas</a></strong></div>
    </div>
</article>
