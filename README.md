lists =a,an,the,as,at,but,by,for,from,in,into,of,on,onto,out,per,to,up,via,with,and,is,are,Series A, Series B, Series C, Series D, Series E

source_list =sec.gov,prnewswire,dowjones,reuters,businesswire,marketwired,fdanews,globenewswire,ema.europa.eu,pwc.com

past_list =has been,have been,is,are,today,Today,announce,announces,will,has,have,now,Now,show,shows,gladly,include,includes,us,Our,our,ours,We,we,may,can,enter,enters,recently,improve,improves,reduce,reduces,decrease,decreases,increase,increases,receive,receives,aim,aims,present,presents,reach,reaches,demonstrate,demonstrates,inhibit,inhibits,induce,induces,plan,plans,continue,continues,provide,provides,covers,cover,do,does,don't,doesn't,reinforce,reinforces,augment,augments,reveal,reveals,inform,informs,conclude,concludes,expect,expects,intend,intends,represent,represents,allege,alleges,allow,allows,indicate,indicates,suggest,suggests,trigger,triggers,grants,believe,believes,anticipate,anticipates,involve,involves,remain,remains,begin,begins,completes,focuses,establishes,give,gives,follow,follows,remove,removes,bind,binds,can't,try,tries,file,files,sign,signs,acquire,acquires,decline,declines,incline,inclines,use,uses,resist,resists,confirm,confirms,means,strengthen,strengthens,support,supports,agree,agrees,enable,enables,report,reports,advise,advises,combines,expand,expands,investigate,investigates,describe,describes,retain,retains,become,becomes,launch,launches,depend,depends,meant of,gather,gathers,accelerate,accelerates,enhance,enhances
	
dictName =we:the Company|We:The Company|is:was|are:were|today:|Today:|announce:announced|announces:announced|will:would|has:had|have:had|now:|Now:|show:showed|shows:showed|gladly:|include:included|includes:included|us:the Company|our:the Company's|Our:The Company's|ours:the Company's|may:might|can:could|enter:entered|enters:entered|recently:|improve:improved|improves:improved|reduce:reduced|reduces:reduced|decrease:decreased|decreases:decreased|increase:increased|increases:increased|receive:received|receives:received|aim:aimed|aims:aimed|present:presented|presents:presented|reach:reached|reaches:reached|has been:was|have been:were|demonstrate:demonstrated|demonstrates:demonstrated|inhibit:inhibited|inhibits:inhibited|induce:induced|induces:induced|plan:planned|plans:planned|continue:continued|continues:continued|provide:provided|provides:provided|cover:covered|covers:covered|do:did|does:did|don't:didn't|doesn't:didn't|reinforce:reinforced|reinforces:reinforced|augment:augmented|augments:augmented|reveal:revealed|reveals:revealed|inform:informed|informs:informed|conclude:concluded|concludes:concluded|expect:expected|expects:expected|intend:intended|intends:intended|represent:represented|represents:represented|allege:alleged|alleges:alleged|indicate:indicated|indicates:indicated|suggest:suggested|suggests:suggested|allow:allowed|allows:allowed|would allowed:would allow|trigger:triggered|triggers:triggered|grants:granted|believe:believed|believes:believed|anticipate:anticipated|anticipates:anticipated|involve:involved|involves:involved|remain:remained|remains:remained|begin:began|begins:began|completes:completed|use:used|uses:used|focuses:focused|establishes:established|give:gave|gives:gave|follow:followed|follows:followed|remove:removed|removes:removed|bind:bound|binds:bound|can't:couldn't|try:tried|tries:tried|file:filed|files:filed|sign:signed|signs:signed|acquire:acquired|acquires:acquired|decline:declined|declines:declined|incline:inclined|inclines:inclined|resist:resisted|resists:resisted|confirm:confirmed|confirms:confirmed|means:meant|strengthen:strengthened|strengthens:strengthened|support:supported|supports:supported|agree:agreed|agrees:agreed|enable:enabled|enables:enabled|report:reported|reports:reported|advise:advised|advises:advised|combines:combined|expand:expanded|expands:expanded|investigate:investigated|investigates:investigated|describe:described|describes:described|retain:retained|retains:retained|become:became|becomes:became|launch:launched|launches:launched|depend:depended|depends:depended|meant of:means of|gather:gathered|gathers:gathered|accelerate:accelerated|accelerates:accelerated|enhance:enhanced|enhances:enhance|

sec_list =We,we,us,Our,our,ours
sec_dict =we:the Company|We:The Company|us:the Company|Our:The Company's|our:the Company's|ours:the Company's|

tickers =NASDAQ,asdaq,TSX,NYSE,TSE,ASX,AMEX,CNQ,LON,OFEX,SEO,GWP,LSE,KOSDAQ,osdaq,KDQ,JASDAQ,HKG,CSE,OTC,OSE,TASE,JSE,AIM,Euronext,Frankfurt Stock,ISIN,EURONEXT,Swiss Exchange,Neuer Markt,"Company"

people_news_keys =( appoint| name| hiring | hires | chief [a-z]+ officer|management changes|leadership|management team)

people_news_keys1 =(management changes|leadership|management team|executive team)

people_news_keys2 =( appoint| name| hiring | hires |new |promote|join| leave| left | bec(o|a)me|transition)

people_news_keys3 =(chief [a-z]+ officer|president| c[a-z]o)

legal_news_keys =( suit | litigat| court| infring| settle| lawsuit| sue| case| invalid| dispute| ruling|appeal)

other_news_keys1 =( facilities| facility| site| office| center| lab| plant|address)

other_news_keys2 =(new |change| mov| establish| expan| open| FDA | GMP |inspect)

remove_event_string =glad to, is pleased to, are pleased to, is delighted to, are delighted to

; (1-2) remove a/an in between a , (3) remove ("takeda") etc, (4) remove (the "company") etc
remove_event_regex_w_case =,(\s?a|\s?an|\s?the)\s([^ ]+\s){0,5}(company|leader|leading)[^,.]*,___,[^,]*(dedicated to|head office|headquarter)[^,.]*,___\s?\(['“”\x{0022}\x{201C}\x{201D}][^\(]*['“”\x{0022}\x{201C}\x{201D}]\)___\s?\([^\(]*the? ?['“”\x{0022}\x{201C}\x{201D}]?Company['“”\x{0022}\x{201C}\x{201D}]?[^\(]*\)

; remove (the "company") etc
remove_event_regex_no_case =\([^\(]*(head office|headquarters|location:|hereafter|CEO|president)[^\(]*\)

verb_protect =( would | wouldn't | will | won't | to | can | can't | could | couldn't | may | might | the |The | also | for | a \S+ \S+? | an \S+ \S+? | A \S+ \S+? |An \S+ \S+? | the \S+ \S+? |The \S+ \S+? )(\S*)
