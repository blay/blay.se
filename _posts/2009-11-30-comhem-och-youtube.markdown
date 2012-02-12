--- 
wordpress_id: 571
layout: post
title: Comhem och youtube
date: 2009-11-30 19:33:00 +01:00
wordpress_url: http://www.blay.se/?p=571
---
Detta känns konstigt. En statisk post om att en dynamisk etherpad har startats. Hursomhelst så utreds just nu <a href="http://img.telecomix.org/EU/src/125956305394.jpg">comhems koppling till youtube</a> av telecomix. Detta flikade jag in i etherpaden. Ändra gärna där istället för att kommentera här :)

http://etherpad.com/comhemyoutube
<div id="magicdomid15" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Scenario:</span></div>
<div id="magicdomid38" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Comhem peerar med google.</span></div>
<div id="magicdomid52" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Vad är peering?</span></div>
<div id="magicdomid54" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9 url"><a href="http://blogs.broughturner.com/2009/04/youtubes-fine-analysts-dont-understand-internet-peering.html">http://blogs.broughturner.com/2009/04/youtubes-fine-analysts-dont-understand-internet-peering.html</a></span></div>
<div id="magicdomid56" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9 url"><a href="http://en.wikipedia.org/wiki/Peering">http://en.wikipedia.org/wiki/Peering</a></span></div>
<div id="magicdomid152" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Internet består som namnet antyder av flera nät. Vi har comhem-nätet, telia-nätet osv.</span></div>
<div id="magicdomid169" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Det finns tre sätt att byta trafik mellan dessa nät. </span></div>
<div id="magicdomid250" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Transit - du "hyr plats" på en annan ISPs nät.</span></div>
<div id="magicdomid343" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">IX - Internet Exchange Point. Plats där ISPar byter trafik mellan varandras nät och betalar beroende på datavolym.</span></div>
<div id="magicdomid344" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Peering &lt;-- det vi är intresserade av här</span></div>
<div id="magicdomid626" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Istället för att gå från punkt A till punkt B via transit (och därmed betala) skapar man en direktlänk. Går det mycket data mellan två punkter är det här bra för då slipper man betala transitavgiften. Exempelvis kanske comhem har peering med bahnhof och skickar då all trafik direkt till bahnhof-länken istället för till IX där det kostar stash.</span></div>
<div id="magicdomid656" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Vänta nu, menar vi fysiska kablar?</span></div>
<div id="magicdomid750" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Nja, man köper/hyr en frekvens i en fiberkabel (ja, en färg faktiskt om man ser det rent fysiskt).</span></div>
<div id="magicdomid770" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Gör Google detta?</span></div>
<div id="magicdomid1199" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Jo, Google är faktiskt en nätleverantör förutom att vara en tjänsteleverantör (detta gör det hela lite klurigt). Så istället för att comhem kör google-trafik över, säg teliasonera, så kan de köra direkt till google-länken. Detta är troligen vad de har gjort.</span></div>
<div id="magicdomid965" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Edge-chaching</span></div>
<div id="magicdomid1166" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Google kör också med edge-caching, vilket innebär att man ställer en burk i ett datacenter som har cache på populär data. Den här cachen kan sen ISPer hyra in sig på. </span></div>
<div id="magicdomid999" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9 url"><a href="http://blogs.broughturner.com/2009/04/googles-peering-and-caching-strategy.html">http://blogs.broughturner.com/2009/04/googles-peering-and-caching-strategy.html</a></span></div>
<div id="magicdomid1220" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Pengar vs. hastighet?</span></div>
<div id="magicdomid1470" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Ovanstående åtgärden innebär i praktiken bara att comhem inte behöver betala lika mycket (till exempelvis telia) och påverkar inte slutkundens prestanda direkt. Dock håller sig google-länken frisk även om en annan koppling (antingen transit eller annan peering) skulle gå ner.</span></div>
<div id="magicdomid1502" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Nätets  utbyggdnad &lt;--- problem</span></div>
<div id="magicdomid1805" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Nätet måste hela tiden byggas ut när trafikmängden och kraven ökar. Med peering och caching direk ttill tjänsteleverantörer kan det innebära att internet byggs ut tjänst för tjänst snarare än "genrellt". Innebär detta endast en avlastning på övrig trafik (ja, delvis) eller kan man också se det som att vissa tjänster prioriteras över andra?</span></div>
<div id="magicdomid1825" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Ny Grej</span></div>
<div id="magicdomid2004" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Allt detta är relativt nytt. Inte så många tjänsteleverantörer kör också nätleverans (telia hostar dock wow, lite samma sak). Så det är värt att tänka över vad detta betyder för internets framtid och om det finns andra alternativ.</span></div>
<div id="magicdomid2025" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Generella cachar:</span></div>
<div id="magicdomid2269" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">En variant är att ISPar bygger (eller köper) generella cachar som cachar poppis material snarare än material från en viss tjänsteleverantör som google. Exempel finns på den israeliska ISPen som började chacha torrent-trafik. Gissningsvis inte poppis hos mediebolagen.</span></div>
<div id="magicdomid2295" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Googles förhandlingsläge:</span></div>
<div id="magicdomid2484" class="ace-line"><span class="author-g-87yqhpnr7vmbmfn9">Google står för enormt stor del av internettrafiken. Vilket förhandlingsläge har de? Alla kommer vilja peera med dem snarare än att köpa google-trafik från någon annan. Kan de förbjuda en ISP att peera med andra tjänsteleverantörer?</span></div>
