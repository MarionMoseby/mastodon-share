Mastodon Share Buttons
===

Share buttons for Mastodon that work on static pages. The page title and URL are pulled from `document.title` and `location.href`, copying the behavior of www.addtoany.com. I've included two options: one for embedding all additional JS/CSS (for security reasons), and another for linking to the JS/CSS hosted here via https://rawgit.com.

Contributions are welcome!

![](screenshot.png)

Demo: https://grayleonard/mastodon-share/demo.html



Instructions
===

To embed without external references:

Large:
```
<div class="mast-share mast-share-lg"><input type="checkbox" class="mast-check-toggle"><div class="mast-instance"><span>Instance: </span><input type="textbox" name="mast-instance-input" placeholder="mastodon.social"><button class="mast-share-button">Share</button></div><label class="mast-top mast-check-label"><span>Share on</span> <img src="data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%20713%20176%22%20height%3D%22188%22%20width%3D%22761%22%3E%0A%20%20%3Cpath%20d%3D%22M161%20105c-3%2013-22%2026-44%2029-12%201-23%203-35%202-20-1-35-5-35-5v6c3%2019%2019%2021%2035%2021%2016%201%2031-4%2031-4v15s-11%206-31%207c-11%200-25-1-41-5-34-9-40-46-41-83V58C0%2020%2025%208%2025%208c13-5%2034-8%2057-8s44%203%2057%208c0%200%2025%2012%2025%2050%200%200%200%2028-3%2047%22%20fill%3D%22%233088d4%22%2F%3E%0A%20%20%3Cpath%20d%3D%22M35%2048a10%2010%200%201%201%2020%200%2010%2010%200%200%201-20%200m144%2013v46h-18V62c0-9-4-14-12-14-9%200-14%205-14%2017v24h-18V65c0-12-4-17-13-17-8%200-12%205-12%2014v45H74V61c0-10%202-17%207-23%205-5%2012-8%2020-8%209%200%2016%203%2021%2011l4%207%205-7c5-8%2012-11%2021-11%208%200%2015%203%2020%208%204%206%207%2013%207%2023m63%2023c4-4%206-9%206-15s-2-11-6-15-8-6-14-6-10%202-14%206c-3%204-5%209-5%2015s2%2011%205%2015c4%204%208%205%2014%205s10-1%2014-5m6-52h18v74h-18v-9c-6%207-14%2011-23%2011-10%200-18-4-24-12-7-7-10-16-10-27s3-21%2010-28c6-8%2014-11%2024-11%209%200%2017%203%2023%2010v-8zm78%2035c6%204%208%2010%208%2017s-3%2013-8%2018c-5%204-12%206-20%206-14%200-24-6-29-18l15-9c2%206%207%209%2014%209%206%200%2010-2%2010-6%200-3-5-6-13-8l-8-3-8-4c-5-4-7-9-7-16s2-13%207-17%2012-6%2019-6c12%200%2021%205%2027%2015l-16%209c-2-5-6-7-11-7s-8%202-8%206c0%203%204%206%2013%208%206%201%2011%203%2015%206m58-17h-16v31c0%203%201%206%204%207h12v18c-13%201-21%200-27-4-5-4-7-11-7-21V50h-12V32h12V17l18-6v21h16v18zm57%2033c4-4%206-9%206-14%200-6-2-11-6-15s-8-6-13-6c-6%200-10%202-14%206s-5%209-5%2015c0%205%201%2010%205%2014s8%206%2014%206c5%200%209-2%2013-6m-40%2013c-7-7-10-16-10-27s3-21%2010-28c7-8%2016-11%2027-11%2010%200%2019%203%2026%2011%207%207%2011%2017%2011%2028s-4%2020-11%2027c-7%208-16%2012-26%2012-11%200-20-4-27-12m124-12c4-4%205-9%205-15s-1-11-5-15-8-6-14-6-10%202-14%206-5%209-5%2015%201%2011%205%2015%209%205%2014%205c6%200%2010-1%2014-5m5-82h18v104h-18v-9c-5%207-12%2011-22%2011s-18-4-24-12c-7-7-10-16-10-27s3-21%2010-28c6-8%2014-11%2024-11s17%203%2022%2010V2zm82%2081c3-4%205-9%205-14%200-6-2-11-5-15-4-4-8-6-14-6-5%200-10%202-13%206-4%204-6%209-6%2015%200%205%202%2010%206%2014%203%204%208%206%2013%206%206%200%2010-2%2014-6m-40%2013c-7-7-11-16-11-27s4-21%2011-28c7-8%2016-11%2026-11%2011%200%2019%203%2027%2011%207%207%2010%2017%2010%2028s-3%2020-10%2027c-8%208-16%2012-27%2012-10%200-19-4-26-12m141-36v46h-18V63c0-5-1-9-3-12-3-2-6-4-11-4-10%200-15%206-15%2019v40h-18V32h18v8c4-7%2011-10%2021-10%208%200%2014%202%2019%208%205%205%207%2013%207%2022%22%20fill%3D%22%23fff%22%2F%3E%0A%3C%2Fsvg%3E%0A"></label></div><script>Array.prototype.forEach||(Array.prototype.forEach=function(r){var o,t;if(null==this)throw new TypeError("this is null or not defined");var n=Object(this),e=n.length>>>0;if("function"!=typeof r)throw new TypeError(r+" is not a function");for(arguments.length>1&&(o=arguments[1]),t=0;t<e;){var i;t in n&&(i=n[t],r.call(o,i,t,n)),t++}});document.addEventListener("DOMContentLoaded",function(){document.querySelectorAll(".mast-share").forEach(function(e,t){e.querySelector(".mast-check-toggle").id="mast-check-toggle-"+t,e.querySelector(".mast-check-label").htmlFor="mast-check-toggle-"+t,e.querySelector(".mast-share-button").addEventListener("click",function(t){var a=new RegExp("^(?:(?:https?|ftp)://)?(?:\\S+(?::\\S*)?@|\\d{1,3}(?:\\.\\d{1,3}){3}|(?:(?:[a-z\\d\\u00a1-\\uffff]+-?)*[a-z\\d\\u00a1-\\uffff]+)(?:\\.(?:[a-z\\d\\u00a1-\\uffff]+-?)*[a-z\\d\\u00a1-\\uffff]+)*(?:\\.[a-z\\u00a1-\\uffff]{2,6}))(?::\\d+)?(?:[^\\s]*)?$","i"),n=e.querySelector('input[name="mast-instance-input"]');if(a.test(n.value)){var o=`http://${n.value.replace(/(^\w+:|^)\/\//,"")}/share?text=${encodeURIComponent(document.title)} ${encodeURIComponent(location.href)}`;window.open(o,"new","toolbar=no,location=no,status=yes,resizable=yes,scrollbars=yes,height=600,width=400")}else n.classList.add("invalid"),setTimeout(function(){n.classList.remove("invalid")},300)}),e.addEventListener("mouseleave",function(t){e.querySelector(".mast-check-toggle").checked=!1})})});</script><style>.mast-check-toggle{height:0;width:0;padding:0;margin:0;visibility:hidden;display:none}.mast-check-toggle:checked+.mast-instance{display:block!important}.mast-check-toggle:not(:checked)+.mast-instance{display:none}.mast-share.active{padding-bottom:10px}.mast-share-lg .mast-top{cursor:pointer;position:absolute;width:142px;top:0;left:0;padding:4px 8px;z-index:1}.mast-share-md .mast-top,.mast-share-sm .mast-top{cursor:pointer;position:absolute;width:18px;height:15px;top:0;left:0;padding:4px 8px;z-index:1}.mast-share-lg,.mast-share-md,.mast-share-sm{color:#fff;display:inline-block;height:23px;background-color:#292D37;border-radius:3px;position:relative}.mast-share-lg{width:158px}.mast-share-md{width:92px}.mast-share-sm{width:34px}.mast-share-md .mast-instance,.mast-share-sm .mast-instance{border-radius:0 3px 3px;z-index:0}.mast-instance{background-color:#292D37;padding:8px;position:absolute;top:20px;left:0;margin:0 auto;border-radius:0 0 3px 3px}.mast-share span{vertical-align:top;font-family:sans-serif;font-weight:700;font-size:14px}.mast-share img{max-height:19px;margin-top:1px}.mast-instance input[name="mast-instance-input"]{background-color:#00000000;border:none;color:#fff;border-bottom:2px solid #3087D5;font-size:14px;font-weight:700;max-width:130px}.mast-instance input[name="mast-instance-input"][class="invalid"]{border-bottom:2px solid red;animation-name:shake;animation-duration:.1s;animation-timing-function:ease-in-out;animation-iteration-count:infinite}@-webkit-keyframes shake{41%,8%{-webkit-transform:translateX(-10px)}25%,58%{-webkit-transform:translateX(10px)}75%{-webkit-transform:translateX(-5px)}92%{-webkit-transform:translateX(5px)}0%,100%{-webkit-transform:translateX(0)}}.mast-share input::placeholder{color:#C7C7CD}.mast-share input:focus{outline:0}.mast-share button{background-color:#00000000;color:#fff;border:none;font-size:14px;font-weight:700;padding:0;margin:8px 0 0;cursor:pointer}.mast-share button:hover{color:#3087d5}</style>
```

Medium: 
```
<div class="mast-share mast-share-md"> <input type="checkbox" class="mast-check-toggle"> <div class="mast-instance"><span>Instance: </span><input type="textbox" name="mast-instance-input" placeholder="mastodon.social"><button class="mast-share-button">Share</button></div> <label class="mast-top mast-check-label"> <img src="data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%20713%20176%22%20height%3D%22188%22%20width%3D%22761%22%3E%0A%20%20%3Cpath%20d%3D%22M161%20105c-3%2013-22%2026-44%2029-12%201-23%203-35%202-20-1-35-5-35-5v6c3%2019%2019%2021%2035%2021%2016%201%2031-4%2031-4v15s-11%206-31%207c-11%200-25-1-41-5-34-9-40-46-41-83V58C0%2020%2025%208%2025%208c13-5%2034-8%2057-8s44%203%2057%208c0%200%2025%2012%2025%2050%200%200%200%2028-3%2047%22%20fill%3D%22%233088d4%22%2F%3E%0A%20%20%3Cpath%20d%3D%22M35%2048a10%2010%200%201%201%2020%200%2010%2010%200%200%201-20%200m144%2013v46h-18V62c0-9-4-14-12-14-9%200-14%205-14%2017v24h-18V65c0-12-4-17-13-17-8%200-12%205-12%2014v45H74V61c0-10%202-17%207-23%205-5%2012-8%2020-8%209%200%2016%203%2021%2011l4%207%205-7c5-8%2012-11%2021-11%208%200%2015%203%2020%208%204%206%207%2013%207%2023m63%2023c4-4%206-9%206-15s-2-11-6-15-8-6-14-6-10%202-14%206c-3%204-5%209-5%2015s2%2011%205%2015c4%204%208%205%2014%205s10-1%2014-5m6-52h18v74h-18v-9c-6%207-14%2011-23%2011-10%200-18-4-24-12-7-7-10-16-10-27s3-21%2010-28c6-8%2014-11%2024-11%209%200%2017%203%2023%2010v-8zm78%2035c6%204%208%2010%208%2017s-3%2013-8%2018c-5%204-12%206-20%206-14%200-24-6-29-18l15-9c2%206%207%209%2014%209%206%200%2010-2%2010-6%200-3-5-6-13-8l-8-3-8-4c-5-4-7-9-7-16s2-13%207-17%2012-6%2019-6c12%200%2021%205%2027%2015l-16%209c-2-5-6-7-11-7s-8%202-8%206c0%203%204%206%2013%208%206%201%2011%203%2015%206m58-17h-16v31c0%203%201%206%204%207h12v18c-13%201-21%200-27-4-5-4-7-11-7-21V50h-12V32h12V17l18-6v21h16v18zm57%2033c4-4%206-9%206-14%200-6-2-11-6-15s-8-6-13-6c-6%200-10%202-14%206s-5%209-5%2015c0%205%201%2010%205%2014s8%206%2014%206c5%200%209-2%2013-6m-40%2013c-7-7-10-16-10-27s3-21%2010-28c7-8%2016-11%2027-11%2010%200%2019%203%2026%2011%207%207%2011%2017%2011%2028s-4%2020-11%2027c-7%208-16%2012-26%2012-11%200-20-4-27-12m124-12c4-4%205-9%205-15s-1-11-5-15-8-6-14-6-10%202-14%206-5%209-5%2015%201%2011%205%2015%209%205%2014%205c6%200%2010-1%2014-5m5-82h18v104h-18v-9c-5%207-12%2011-22%2011s-18-4-24-12c-7-7-10-16-10-27s3-21%2010-28c6-8%2014-11%2024-11s17%203%2022%2010V2zm82%2081c3-4%205-9%205-14%200-6-2-11-5-15-4-4-8-6-14-6-5%200-10%202-13%206-4%204-6%209-6%2015%200%205%202%2010%206%2014%203%204%208%206%2013%206%206%200%2010-2%2014-6m-40%2013c-7-7-11-16-11-27s4-21%2011-28c7-8%2016-11%2026-11%2011%200%2019%203%2027%2011%207%207%2010%2017%2010%2028s-3%2020-10%2027c-8%208-16%2012-27%2012-10%200-19-4-26-12m141-36v46h-18V63c0-5-1-9-3-12-3-2-6-4-11-4-10%200-15%206-15%2019v40h-18V32h18v8c4-7%2011-10%2021-10%208%200%2014%202%2019%208%205%205%207%2013%207%2022%22%20fill%3D%22%23fff%22%2F%3E%0A%3C%2Fsvg%3E%0A"> </label> </div> <script>Array.prototype.forEach||(Array.prototype.forEach=function(r){var o,t;if(null==this)throw new TypeError("this is null or not defined");var n=Object(this),e=n.length>>>0;if("function"!=typeof r)throw new TypeError(r+" is not a function");for(arguments.length>1&&(o=arguments[1]),t=0;t<e;){var i;t in n&&(i=n[t],r.call(o,i,t,n)),t++}});document.addEventListener("DOMContentLoaded",function(){document.querySelectorAll(".mast-share").forEach(function(e,t){e.querySelector(".mast-check-toggle").id="mast-check-toggle-"+t,e.querySelector(".mast-check-label").htmlFor="mast-check-toggle-"+t,e.querySelector(".mast-share-button").addEventListener("click",function(t){var a=new RegExp("^(?:(?:https?|ftp)://)?(?:\\S+(?::\\S*)?@|\\d{1,3}(?:\\.\\d{1,3}){3}|(?:(?:[a-z\\d\\u00a1-\\uffff]+-?)*[a-z\\d\\u00a1-\\uffff]+)(?:\\.(?:[a-z\\d\\u00a1-\\uffff]+-?)*[a-z\\d\\u00a1-\\uffff]+)*(?:\\.[a-z\\u00a1-\\uffff]{2,6}))(?::\\d+)?(?:[^\\s]*)?$","i"),n=e.querySelector('input[name="mast-instance-input"]');if(a.test(n.value)){var o=`http://${n.value.replace(/(^\w+:|^)\/\//,"")}/share?text=${encodeURIComponent(document.title)} ${encodeURIComponent(location.href)}`;window.open(o,"new","toolbar=no,location=no,status=yes,resizable=yes,scrollbars=yes,height=600,width=400")}else n.classList.add("invalid"),setTimeout(function(){n.classList.remove("invalid")},300)}),e.addEventListener("mouseleave",function(t){e.querySelector(".mast-check-toggle").checked=!1})})});</script> <style>.mast-check-toggle{height:0;width:0;padding:0;margin:0;visibility:hidden;display:none}.mast-check-toggle:checked+.mast-instance{display:block!important}.mast-check-toggle:not(:checked)+.mast-instance{display:none}.mast-share.active{padding-bottom:10px}.mast-share-lg .mast-top{cursor:pointer;position:absolute;width:142px;top:0;left:0;padding:4px 8px;z-index:1}.mast-share-md .mast-top,.mast-share-sm .mast-top{cursor:pointer;position:absolute;width:18px;height:15px;top:0;left:0;padding:4px 8px;z-index:1}.mast-share-lg,.mast-share-md,.mast-share-sm{color:#fff;display:inline-block;height:23px;background-color:#292D37;border-radius:3px;position:relative}.mast-share-lg{width:158px}.mast-share-md{width:92px}.mast-share-sm{width:34px}.mast-share-md .mast-instance,.mast-share-sm .mast-instance{border-radius:0 3px 3px;z-index:0}.mast-instance{background-color:#292D37;padding:8px;position:absolute;top:20px;left:0;margin:0 auto;border-radius:0 0 3px 3px}.mast-share span{vertical-align:top;font-family:sans-serif;font-weight:700;font-size:14px}.mast-share img{max-height:19px;margin-top:1px}.mast-instance input[name="mast-instance-input"]{background-color:#00000000;border:none;color:#fff;border-bottom:2px solid #3087D5;font-size:14px;font-weight:700;max-width:130px}.mast-instance input[name="mast-instance-input"][class="invalid"]{border-bottom:2px solid red;animation-name:shake;animation-duration:.1s;animation-timing-function:ease-in-out;animation-iteration-count:infinite}@-webkit-keyframes shake{41%,8%{-webkit-transform:translateX(-10px)}25%,58%{-webkit-transform:translateX(10px)}75%{-webkit-transform:translateX(-5px)}92%{-webkit-transform:translateX(5px)}0%,100%{-webkit-transform:translateX(0)}}.mast-share input::placeholder{color:#C7C7CD}.mast-share input:focus{outline:0}.mast-share button{background-color:#00000000;color:#fff;border:none;font-size:14px;font-weight:700;padding:0;margin:8px 0 0;cursor:pointer}.mast-share button:hover{color:#3087d5}</style>
```

Small:
```
<div class="mast-share mast-share-sm"> <input type="checkbox" class="mast-check-toggle"> <div class="mast-instance"><span>Instance: </span><input type="textbox" name="mast-instance-input" placeholder="mastodon.social"><button class="mast-share-button">Share</button></div> <label class="mast-top mast-check-label"> <img src="data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20width%3D%2261.076954mm%22%20height%3D%2265.47831mm%22%20viewBox%3D%220%200%20216.4144%20232.00976%22%3E%3Cpath%20d%3D%22M211.80734%20139.0875c-3.18125%2016.36625-28.4925%2034.2775-57.5625%2037.74875-15.15875%201.80875-30.08375%203.47125-45.99875%202.74125-26.0275-1.1925-46.565-6.2125-46.565-6.2125%200%202.53375.15625%204.94625.46875%207.2025%203.38375%2025.68625%2025.47%2027.225%2046.39125%2027.9425%2021.11625.7225%2039.91875-5.20625%2039.91875-5.20625l.8675%2019.09s-14.77%207.93125-41.08125%209.39c-14.50875.7975-32.52375-.365-53.50625-5.91875C9.23234%20213.82%201.40609%20165.31125.20859%20116.09125c-.365-14.61375-.14-28.39375-.14-39.91875%200-50.33%2032.97625-65.0825%2032.97625-65.0825C49.67234%203.45375%2078.20359.2425%20107.86484%200h.72875c29.66125.2425%2058.21125%203.45375%2074.8375%2011.09%200%200%2032.975%2014.7525%2032.975%2065.0825%200%200%20.41375%2037.13375-4.59875%2062.915%22%20fill%3D%22%233088d4%22%2F%3E%3Cpath%20d%3D%22M177.50984%2080.077v60.94125h-24.14375v-59.15c0-12.46875-5.24625-18.7975-15.74-18.7975-11.6025%200-17.4175%207.5075-17.4175%2022.3525v32.37625H96.20734V85.42325c0-14.845-5.81625-22.3525-17.41875-22.3525-10.49375%200-15.74%206.32875-15.74%2018.7975v59.15H38.90484V80.077c0-12.455%203.17125-22.3525%209.54125-29.675%206.56875-7.3225%2015.17125-11.07625%2025.85-11.07625%2012.355%200%2021.71125%204.74875%2027.8975%2014.2475l6.01375%2010.08125%206.015-10.08125c6.185-9.49875%2015.54125-14.2475%2027.8975-14.2475%2010.6775%200%2019.28%203.75375%2025.85%2011.07625%206.36875%207.3225%209.54%2017.22%209.54%2029.675%22%20fill%3D%22%23fff%22%2F%3E%3C%2Fsvg%3E%0A"> </label> </div> <script>Array.prototype.forEach||(Array.prototype.forEach=function(r){var o,t;if(null==this)throw new TypeError("this is null or not defined");var n=Object(this),e=n.length>>>0;if("function"!=typeof r)throw new TypeError(r+" is not a function");for(arguments.length>1&&(o=arguments[1]),t=0;t<e;){var i;t in n&&(i=n[t],r.call(o,i,t,n)),t++}});document.addEventListener("DOMContentLoaded",function(){document.querySelectorAll(".mast-share").forEach(function(e,t){e.querySelector(".mast-check-toggle").id="mast-check-toggle-"+t,e.querySelector(".mast-check-label").htmlFor="mast-check-toggle-"+t,e.querySelector(".mast-share-button").addEventListener("click",function(t){var a=new RegExp("^(?:(?:https?|ftp)://)?(?:\\S+(?::\\S*)?@|\\d{1,3}(?:\\.\\d{1,3}){3}|(?:(?:[a-z\\d\\u00a1-\\uffff]+-?)*[a-z\\d\\u00a1-\\uffff]+)(?:\\.(?:[a-z\\d\\u00a1-\\uffff]+-?)*[a-z\\d\\u00a1-\\uffff]+)*(?:\\.[a-z\\u00a1-\\uffff]{2,6}))(?::\\d+)?(?:[^\\s]*)?$","i"),n=e.querySelector('input[name="mast-instance-input"]');if(a.test(n.value)){var o=`http://${n.value.replace(/(^\w+:|^)\/\//,"")}/share?text=${encodeURIComponent(document.title)} ${encodeURIComponent(location.href)}`;window.open(o,"new","toolbar=no,location=no,status=yes,resizable=yes,scrollbars=yes,height=600,width=400")}else n.classList.add("invalid"),setTimeout(function(){n.classList.remove("invalid")},300)}),e.addEventListener("mouseleave",function(t){e.querySelector(".mast-check-toggle").checked=!1})})});</script> <style>.mast-check-toggle{height:0;width:0;padding:0;margin:0;visibility:hidden;display:none}.mast-check-toggle:checked+.mast-instance{display:block!important}.mast-check-toggle:not(:checked)+.mast-instance{display:none}.mast-share.active{padding-bottom:10px}.mast-share-lg .mast-top{cursor:pointer;position:absolute;width:142px;top:0;left:0;padding:4px 8px;z-index:1}.mast-share-md .mast-top,.mast-share-sm .mast-top{cursor:pointer;position:absolute;width:18px;height:15px;top:0;left:0;padding:4px 8px;z-index:1}.mast-share-lg,.mast-share-md,.mast-share-sm{color:#fff;display:inline-block;height:23px;background-color:#292D37;border-radius:3px;position:relative}.mast-share-lg{width:158px}.mast-share-md{width:92px}.mast-share-sm{width:34px}.mast-share-md .mast-instance,.mast-share-sm .mast-instance{border-radius:0 3px 3px;z-index:0}.mast-instance{background-color:#292D37;padding:8px;position:absolute;top:20px;left:0;margin:0 auto;border-radius:0 0 3px 3px}.mast-share span{vertical-align:top;font-family:sans-serif;font-weight:700;font-size:14px}.mast-share img{max-height:19px;margin-top:1px}.mast-instance input[name="mast-instance-input"]{background-color:#00000000;border:none;color:#fff;border-bottom:2px solid #3087D5;font-size:14px;font-weight:700;max-width:130px}.mast-instance input[name="mast-instance-input"][class="invalid"]{border-bottom:2px solid red;animation-name:shake;animation-duration:.1s;animation-timing-function:ease-in-out;animation-iteration-count:infinite}@-webkit-keyframes shake{41%,8%{-webkit-transform:translateX(-10px)}25%,58%{-webkit-transform:translateX(10px)}75%{-webkit-transform:translateX(-5px)}92%{-webkit-transform:translateX(5px)}0%,100%{-webkit-transform:translateX(0)}}.mast-share input::placeholder{color:#C7C7CD}.mast-share input:focus{outline:0}.mast-share button{background-color:#00000000;color:#fff;border:none;font-size:14px;font-weight:700;padding:0;margin:8px 0 0;cursor:pointer}.mast-share button:hover{color:#3087d5}</style>
```

To embed with external network calls (hosted on jsdelivr):

Large:
```
<div class="mast-share mast-share-lg"> <input type="checkbox" class="mast-check-toggle"> <div class="mast-instance"><span>Instance: </span><input type="textbox" name="mast-instance-input" placeholder="mastodon.social"><button class="mast-share-button">Share</button></div> <label class="mast-top mast-check-label"> <span>Share on</span> <img src="logotype-full.svg"> </label> </div> <script src="https://cdn.rawgit.com/grayleonard/mastodon-share/35d4e3ab/mast-share.min.js"></script> <link rel="stylesheet" href="https://cdn.rawgit.com/grayleonard/mastodon-share/35d4e3ab/mast-share.min.css">
```

Medium:
```
<div class="mast-share mast-share-md"> <input type="checkbox" class="mast-check-toggle"> <div class="mast-instance"><span>Instance: </span><input type="textbox" name="mast-instance-input" placeholder="mastodon.social"><button class="mast-share-button">Share</button></div> <label class="mast-top mast-check-label"> <img src="logotype-full.svg"> </label> </div> <script src="https://cdn.rawgit.com/grayleonard/mastodon-share/35d4e3ab/mast-share.min.js"></script> <link rel="stylesheet" href="https://cdn.rawgit.com/grayleonard/mastodon-share/35d4e3ab/mast-share.min.css">
```


Small:
```
<div class="mast-share mast-share-sm"> <input type="checkbox" class="mast-check-toggle"> <div class="mast-instance"><span>Instance: </span><input type="textbox" name="mast-instance-input" placeholder="mastodon.social"><button class="mast-share-button">Share</button></div> <label class="mast-top mast-check-label"> <img src="logotype-short.svg"> </label> </div> <script src="https://cdn.rawgit.com/grayleonard/mastodon-share/35d4e3ab/mast-share.min.js"></script> <link rel="stylesheet" href="https://cdn.rawgit.com/grayleonard/mastodon-share/35d4e3ab/mast-share.min.css">
```