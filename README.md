# Stochastic epidemiological models to test the origin and demographic impact of smallpox on Aboriginal Australians in the 18<sup>th</sup> Century
<img align="right" src="www/smallpox.png" width="200" style="margin-top: 20px">

## Focal manuscript
<a href="https://www.flinders.edu.au/people/cody.nitschke">Nitschke, MC</a>, <a href="https://au.linkedin.com/in/alan-williams-7973a958">AN Williams</a>, <a href="https://scholars.uow.edu.au/shane-ingrey">SD Ingrey</a>, <a href="https://experts.deakin.edu.au/42085-billy-griffiths">B Griffiths</a>, <a href="https://au.linkedin.com/in/nick-pitt-772440ba">N Pitt</a>, <a href="https://research.monash.edu/en/persons/lynette-russell-am">L Russell</a>, <a href="https://portfolio.jcu.edu.au/researchers/sean.ulm/">S Ulm</a>, <a href="https://www.facebook.com/profile.php?id=100076324899510">K Beller</a>, <a href="https://research.unsw.edu.au/people/dr-jarrod-ray-hore">JR Hore</a>, <a href="https://portfolio.jcu.edu.au/researchers/michael.bird">MI Bird</a>, <a href="https://globalecologyflinders.com/people/#SHF">SH Fatima</a>, <a href="https://research.monash.edu/en/persons/ian-mcniven">IJ McNiven</a>, <a href="https://www.flinders.edu.au/people/frederik.saltre">F Saltré</a>, <a href="https://www.unsw.edu.au/staff/alison-bashford">A Bashford</a>, <a href="https://discover.utas.edu.au/Christopher.Wilson">C Wilson</a>, <a href="https://www.flinders.edu.au/people/corey.bradshaw">CJA Bradshaw</a>. <a href="">Stochastic models indicate rapid smallpox spread and mass mortality of Indigenous Australians after colonial exposure</a>. In review

## Abstract
The impact of smallpox (variola) on Aboriginal peoples of Australia in 1789 was catastrophic and irreversible. Historically biased perspectives of the disease’s introduction and spread impede modern-day reconciliation efforts. Understanding whether the disease entered and spread from pre-colonial Makassan (Indonesian) trade along the north coast, or from the First Fleet’s arrival in south-eastern Australia is necessary to infer the likely rate of spread and magnitude of mortality. We developed stochastic, multi-patch epidemiological models, supported by historical observations of the disease, to test hypotheses regarding possible entry points, spread rate, and demographic impacts. Our models suggest that entry from south-eastern Australia was more likely, with a probability < 0.02 of reaching Sydney from a northern entry, and an unrealistic chronology. The spread of the disease was rapid, and suggests a single interaction could have resulted in the widespread impacts of the disease. Initial entry to extinction of the disease took between 1,200 and 1,400 days (< 4 years), and due to its high mortality rate, appears to have been limited to the eastern margins of Australia and along major intersecting river systems. There was a lower likelihood of transmission into semi-arid, arid, or tropical areas. We found no evidence that smallpox would have reached the central or western half of Australia. Assuming a 60% lethality based on global data, the loss of > 150,000 people would have occurred in these regions in < 4 years, more than previously proposed, but in alignment with recent projections of demographic change during that period.

## <a href="https://github.com/mcnitschke/Smallpox-in-Aboriginal-Australia/tree/main/scripts">Scripts</a>
- main script: <code>OneStage.m</code>

### Functions within main script
- <code>Movement1Stage.m</code>: simulates movement between neighbouring patches
- <code>Spread_beta.m</code>: simulates disease spread through contact within each patch (susceptible to exposed; S → E)
- <code>RecoverDeath.m</code>: simulates the other stages of the disease (exposed to infected; E → I and infected to recovered; I → R)

## <a href="https://github.com/mcnitschke/Smallpox-in-Aboriginal-Australia/tree/main/data">Data</a>
- <em>Populations.mat</em>: projected population vector for each patch (1×592)
- <em>Q.mat</em>: conditional probability of movement to each neighbouring patch (∑ for each patch = 1).  
- <em>Tindale.mat</em>: area for each patch based on Tindale map (1940)

### Acknowledgements
We acknowledge the sovereign Traditional Owners and custodians (First Nations) of the unceded lands and seas where we live and work, including <a href="https://www.kaurnawarra.org.au/kaurna-people">Kaurna</a> in Tarndanya/Adelaide (M.C.N., C.J.A.B., F.S., S.H.F.), <a href="https://www.gujaga.org.au/faq">Bidiagal</a> in Warrane/Sydney (A.N.W., N.P., J.R.H., A.B.), <a href="https://www.sutherlandshire.nsw.gov.au/play-and-explore/local-history-and-heritage/local-history">Dharawal</a> in Kamay/Botany Bay (K.B., S.D.I.), <a href="https://www.melbourne.vic.gov.au/aboriginal-melbourne">Kulin</a> Nation in Naarm/Melbourne (B.G., I.J.M., L.R.), <a href="https://dawulwuru.com.au/">Yirrganydji</a> and <a href="https://www.yidinji.com/">Gimuy Walubara Yidinji</a> in Gimuy/Cairns (S.U., M.I.B.), <a href="https://www.sutherlandshire.nsw.gov.au/play-and-explore/local-history-and-heritage/local-history">Dharawal</a> in Woolungah/Wollongong (F.S.), <a href="https://ngarrindjeri.com.au/">Ngarrindjeri</a> of Murrundi/lower Murray River, Kurangk/Coorong, and eastern Fleurieu Peninsula (C.W.), <a href="https://tacinc.com.au/">Palawa</a> in Nipaluna/Hobart, lutruwitra/Tasmania (C.W.), and <a href="https://www.facebook.com/peramangkgovernancecouncil/">Peramangk</a> in Bukatila/Mount Lofty Ranges (C.J.A.B.). We also recognise the deep historical and cultural harm our truth-telling exposes, and we commiserate with all First Nations peoples of Australia. We thank <a href="https://globalecologyflinders.com/people/#JL">J. Llewelyn</a> for initial discussions.

### Funding
Funded jointly by the <a href="http://www.arc.gov.au">Australian Research Council</a> <a href="http://ciehf.au">Centre of Excellence for Indigenous and Environmental Histories and Futures</a> (CE230100009), and the Australian Research Council <a href="http://epicaustralia.org.au">Centre of Excellence for Australian Biodiversity and Heritage</a> (CE17010001). L.R. supported by an Australian Research Council Laureate Fellowship (FL190100161). B.G. supported by an Australian Research Council Discovery Early Career Researcher Award (DE220100203). A.B. and N.P. supported by an Australian Research Council Laureate Fellowship (FL200100144).</br>
<br>
<p><a href="https://www.flinders.edu.au"><img align="bottom-left" src="www/Flinders_University_Logo_Horizontal_RGB_Master.png" alt="Flinders University" height="40" style="margin-top: 20px"></a> <a href="https://globalecologyflinders.com"><img align="bottom-left" src="www/GEL Logo Kaurna New Transp.png" alt="GEL logo" height="55" style="margin-top: 20px"></a> <a href="https://ciehf.au/"><img align="bottom-left" src="www/CIEHF_Logo_Email_Version Transparent.png" alt="CIEHF" height="45" style="margin-top: 20px"></a> <a href="https://epicaustralia.org.au"><img align="bottom-left" src="www/CabahFCL.cropped.jpg" alt="CABAH" height="50" style="margin-top: 20px"></a> &nbsp; <a href="https://www.facebook.com/profile.php?id=100076324899510"><img align="bottom-left" src="www/GujagaFoundation.png" alt="Gujaga Foundation" height="45" style="margin-top: 20px"></a> &nbsp; <a href="https://www.jcu.edu.au/"><img align="bottom-left" src="www/JCULogo.webp" alt="James Cook University" height="45" style="margin-top: 20px"></a> &nbsp; <a href="https://www.unsw.edu.au/"><img align="bottom-left" src="www/UNSWLogo.png" alt="UNSW" height="45" style="margin-top: 20px"></a> &nbsp; <a href="https://www.monash.edu/"><img align="bottom-left" src="www/MonashLogo.webp" alt="Monash University" height="55" style="margin-top: 20px"></a> &nbsp; <a href="https://www.deakin.edu/"><img align="bottom-left" src="www/DeakinULogo.svg" alt="Deakin University" height="45" style="margin-top: 20px"></a> <a href="https://www.utas.edu/"><img align="bottom-left" src="www/UTASLogo.webp" alt="University of Tasmania" height="45" style="margin-top: 20px"></a></p>
