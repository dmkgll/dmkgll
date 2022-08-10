---
layout: index
---

<style>img{max-width:100%;}ul{
    list-style: none;
    padding: 0;
}
body{font-family:sans-serif;font-size:14px;}
 /*@media (min-width: 600px) {
        a:hover:after {
            content: "<--- " attr(data);
            position: absolute;
            background: white;
            color: black;
            padding: 2px 4px;
            margin: -2px 0 0 1px;
        }
  
    }*/
		    
		    h1, h2 {
    /* margin: 1.5em 0 0.5em; */
    font-size: 18px;
    padding: 10px;
    font-family: serif;
    /* text-transform: uppercase; */
    background: yellow;
}
		    
		    p {
    margin: 0.5em 0.5em 1em 1em;
}
		    

</style>

{% assign documents = site.documents | sort: 'date' | reverse %}

{% for document in documents limit:500 %}
  {% if document.layout == 'index' %}
<div class="post-stub">
       <h2>
      <span class="date hidden-xs">{{ document.date | date: "%Y-%m-%d" }}    </span>
             {% if document.layout == "post" %} <span class="title">   <a href="{{ document.url | relative_url }}">{{ document.title }} </a>
         </span>{% elsif document.layout == "link" %} <span class="title">   <a href="{{ document.link | relative_url }}"> {{ document.title }} | {{ document.site }} </a>→
         </span> 
         
        {% else %} <span class="title">   <a href="{{ document.url | relative_url }}">{{ document.date | date: "%H:%M:%S" }}   </a>
         </span>  {% endif %}
       
       
       </h2>
         {% if document.reply %}
 <p><span class="reply-context" style="display:block;background-color: #f5f5f5;text-indent: 1em; line-break:anywhere;">↳ In reply to <a href="{{ document.reply | relative_url }}" class="u-in-reply-to h-cite">{{ document.reply }}</a></span></p>
  {% endif %}
       
       {% if document.layout == "post" %}   <p class="p-content"> {{ document.excerpt  }} </p>     
       {% else %}
       
        <p class="p-content"> 
   {{ document.content | truncate: 445 }}
 </p>
         {% endif %}
       
    {% if document.image %}
      <div class="post-image">
        <a href="{{ document.url | relative_url }}" style="
    text-decoration: none;
">
          <img src="{{ document.image | relative_url }}" alt="{{ document.alt }}" style="max-width:60%">
          
        </a>
       </div>  
       {% endif %}         
         
        
 </div> 
  {% endif %}   
{% endfor %}		    
		    
		    
		    
 <div class="posts">
  {% for post in paginator.posts %}
  <div class="post">
  <h1 class="post-title">
   <a href="{{ post.url }}">
  {{ post.title }}
      </a>
    </h1>
{{ post.content }}
  </div>
  {% endfor %}
</div>
		   
<!---
<ul>
<li><a href="/" data="A parody response to the smug banned books store displays that feature totally uncontroversial books.">Based Penguin Classics</a> <small>2022</small><br>A parody response to the smug "banned books" store displays with uncontroversial books.</li>		    
<li><a href="/" data="a parody of the silly Anticapitalist Software License">The Family of the Vourdalak</a> <small>2022</small><br>My translation of the 1839 vampire short story by Aleksey Tolstoy.</li>
  <li><a href="/" data="a parody of the silly Anticapitalist Software License">Capitalist Software License</a> <small>2022</small></li>
  <li><a href="/doomhearn" data="a parody of the silly Anticapitalist Software License">Doom Hearn</a> <small>2022</small></li>
  <li><a href="/fet" data="blogging project inspired by Kevin Quirk">100 Day Blog</a> <small>2022</small></li>
  <li><a href="/royhol" data="bitcoin fine art project inspired by Andy Warhol and (Dr.) Roy Murphy">Royhol</a> <small>2022</small></li>
  <li><a href="/fet" data="blog featuring the best sci-fi cover art, mostly old">Sci-Fi Covers</a> <small>2022</small></li>
  <li><a href="/fet">First Edition Tees</a> <small>2022</small></li>
  <li><a href="/ayn-rand-ipsum">Ayn Rand Ipsum</a> <small>2022-</small><br>An alternative to the ubiquitous Lorem Ipsum.</li>
  <li><a href="/strangers">I will not argue with strangers on the internet</a> <small>2022-</small></li>
  <li><a href="https://howtokeepanidiotinsuspense.com">How to keep an idiot in suspense</a> <small>2022-</small></li>
  <li><a href="thesoontimes.com">The Soon Times</a> <small>2021-</small><br>Cryptocurrency parody news site.</li>
  <li><a href="thesoontimes.com">Numpty Coin Club Teeshirt</a> <small>2021</small></li>
  <li><a href="/">Twetch Encrypt &amp; Delete + Lock</a> <small>2021</small></li>
  <li><a href="/csw12">Craig Wright’s <em>Twelve Days of Christmas</em></a> <small>2021</small></li>
  <li><a href="/bsvdomains">bitcoinsv.domains</a> <small>2020-2021</small><br>BSV domain squatting site. RIP.</li>
  <li><a href="/pathly">Pathly</a> <small>2018-2019</small></li>
  <li><a href="/v&amp;e">Voice &amp; Exit</a> <small>2016</small><br>Marketing strategy for anarcho-futurist conference in Austin, TX.</li>
  <li><a href="/bvyd">Bindel vs Yiannopoulos Debate</a> <small>2016</small></li>
  <li><a href="/acutuc">(Accidental) Ten Million Dollar Facebook Ad</a> <small>2015</small></li>		    
  <li><a href="/nohipster">No Hipster Stocks</a> <small>2015-2016</small></li>
  <li><a href="/speaking">Speaking</a> <small>2014-2019</small></li>
  <li><a href="https://discoverpraxis.com">Praxis</a> <small>2014-2018</small></li>		    
  <li><a href="/hvk">Hayek v. Keynes</a> <small>2014</small><br>Submission for a libertarian art gala.</li>
  <li><a href="/oldstuff">Old writing</a> <small>2013-2021</small></li>
  <li><a href="/wltops">We Were Promised Laptops</a> <small>2012</small><br>Trolling the highschool admin.</li>
</ul>--->

<p></p>

<!---
- [Twitter](https://twitter.com/dmkgll)
- [Email](/)
- [Featured In](/)
 --->
<img alt="image" loading="lazy" src="/assets/tcb.jpeg" style="max-width: 300px;
">

*["According to the Internet, Deryk occupies every corner of the Nolan chart."](/)*

<img alt="image" loading="lazy" src="/assets/mc.jpeg" style="max-width: 200px;
">

```
+-----------------------------------------------+     
|x o -                              advertisement     
|                                               |     
|    ^_~    DMKGLL.COM IS NOW SELLING           |     
|                ADVERTISING SPACE          *_* |     
| ©     ☭                              :]       |     
|                 YOUR AD HERE                  |     
|    ☉ ‿ ⚆                           ⚂          |     
|          Δ           $                 €      |     
|     ☆                       ✿                 |     
|             ☀                  ☯              |     
+-----------------------------------------------+     
 ```                                                     
                                                      
<img alt="image" loading="lazy" src="/assets/marsjunctionhat.png" style="max-width: 250px;
">                                              

---

<p>
		<a href="https://validator.w3.org/check?uri=https://www.lolwut.info/index.html"><img src="https://anlucas.neocities.org/anow.gif" width="88" height="31" alt="Valid HTML 4.01 Strict" title="Valid HTML 4.01 Strict"></a>
	
<a href="https://twet.ch/inv/400a1db9"><img style="border-bottom: 2px inset rgb(0 0 0);
    border-right: 2px inset rgb(0 0 0);
    box-sizing: border-box;
    color: white;
    cursor: pointer;
    display: inline-block;
	border-top: 1px solid;
    font-size: 2.2rem;" src="/assets/twetch.gif" width="88" height="31" alt="Valid HTML 4.01 Strict" title="Valid HTML 4.01 Strict"></a>
	
<a href="https://twet.ch/inv/400a1db9"><img src="/assets/notoweb3.gif" width="88" height="31" alt="Valid HTML 4.01 Strict" title="Valid HTML 4.01 Strict"></a>
	

</p>

*This page last updated 21 July 2022*
