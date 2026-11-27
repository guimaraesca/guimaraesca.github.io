---
layout: page
title: cases
permalink: /projects/
description: Os cases agora estão organizados por frente na página de consultoria.
nav: false
redirect: /consultoria/
---

<p>Os cases agora estão na página de <a href="{{ '/consultoria/' | relative_url }}">consultoria</a>, organizados por frente.</p>

<script>
(function(){
  var h=decodeURIComponent(location.hash.slice(1)), m={t1:'transformacao-digital',t2:'educacao',t3:'inovacao'};
  var base='{{ "/consultoria/" | relative_url }}', home='{{ "/" | relative_url }}';
  var dest=base;
  if(m[h]) dest=base+'#'+m[h];
  else if(h==='t4'||/^e-(cenep|unifacex|gamedu|ifrn|kroton)/.test(h)) dest=home+'#trajetoria';
  else if(h==='c-6_imd') dest='{{ "/projects/6_imd/" | relative_url }}';
  else if(/^[ce]-/.test(h)) dest=base+'#'+h;
  location.replace(dest);
})();
</script>
