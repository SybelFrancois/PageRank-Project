# PageRank-Project

## Tasks Results

1. Below are the outputs of all the tasks after running each corresponding command (with correct markdown formatting)...
   
   Task 1, part 1:
   ```
   $ python3 pagerank.py --data=data/small.csv.gz --verbose
   DEBUG:root:computing indices
   DEBUG:root:computing values
   DEBUG:root:i=0 residual=0.3517141342163086
   DEBUG:root:i=1 residual=0.21420912444591522
   DEBUG:root:i=2 residual=0.11156422644853592
   DEBUG:root:i=3 residual=0.04077015444636345
   DEBUG:root:i=4 residual=0.022621305659413338
   DEBUG:root:i=5 residual=0.008656897582113743
   DEBUG:root:i=6 residual=0.0046537392772734165
   DEBUG:root:i=7 residual=0.00189716718159616
   DEBUG:root:i=8 residual=0.0009609037078917027
   DEBUG:root:i=9 residual=0.0004073376767337322
   DEBUG:root:i=10 residual=0.00019723437435459346
   DEBUG:root:i=11 residual=8.549748599762097e-05
   DEBUG:root:i=12 residual=4.018686377094127e-05
   DEBUG:root:i=13 residual=1.759403312462382e-05
   DEBUG:root:i=14 residual=8.092925781966187e-06
   DEBUG:root:i=15 residual=3.5313314583618194e-06
   DEBUG:root:i=16 residual=1.5786969242981286e-06
   DEBUG:root:i=17 residual=6.826130629633553e-07
   INFO:root:rank=0 pagerank=7.1066e-01 url=4
   INFO:root:rank=1 pagerank=5.4547e-01 url=6
   INFO:root:rank=2 pagerank=4.0102e-01 url=5
   INFO:root:rank=3 pagerank=1.3243e-01 url=2
   INFO:root:rank=4 pagerank=1.0269e-01 url=3
   INFO:root:rank=5 pagerank=9.2326e-02 url=1
   ```

   Task 1, part 2:
   ```
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='corona'
   INFO:root:rank=0 pagerank=1.0038e-03 url=www.lawfareblog.com/lawfare-podcast-united-nations-and-coronavirus-crisis
   INFO:root:rank=1 pagerank=8.9228e-04 url=www.lawfareblog.com/house-oversight-committee-holds-day-two-hearing-government-coronavirus-response
   INFO:root:rank=2 pagerank=7.0394e-04 url=www.lawfareblog.com/britains-coronavirus-response
   INFO:root:rank=3 pagerank=6.9157e-04 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
   INFO:root:rank=4 pagerank=6.7045e-04 url=www.lawfareblog.com/israeli-emergency-regulations-location-tracking-coronavirus-carriers
   INFO:root:rank=5 pagerank=6.6260e-04 url=www.lawfareblog.com/why-congress-conducting-business-usual-face-coronavirus
   INFO:root:rank=6 pagerank=6.5050e-04 url=www.lawfareblog.com/congressional-homeland-security-committees-seek-ways-support-state-federal-responses-coronavirus
   INFO:root:rank=7 pagerank=6.3623e-04 url=www.lawfareblog.com/paper-hearing-experts-debate-digital-contact-tracing-and-coronavirus-privacy-concerns
   INFO:root:rank=8 pagerank=6.1252e-04 url=www.lawfareblog.com/house-subcommittee-voices-concerns-over-us-management-coronavirus
   INFO:root:rank=9 pagerank=6.0191e-04 url=www.lawfareblog.com/livestream-house-oversight-committee-holds-hearing-government-coronavirus-response

   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='trump'
   INFO:root:rank=0 pagerank=5.7827e-03 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
   INFO:root:rank=1 pagerank=5.2340e-03 url=www.lawfareblog.com/document-trump-revokes-obama-executive-order-counterterrorism-strike-casualty-reporting
   INFO:root:rank=2 pagerank=5.1298e-03 url=www.lawfareblog.com/trump-administrations-worrying-new-policy-israeli-settlements
   INFO:root:rank=3 pagerank=4.6601e-03 url=www.lawfareblog.com/dc-circuit-overrules-district-courts-due-process-ruling-qasim-v-trump
   INFO:root:rank=4 pagerank=4.5935e-03 url=www.lawfareblog.com/donald-trump-and-politically-weaponized-executive-branch
   INFO:root:rank=5 pagerank=4.3073e-03 url=www.lawfareblog.com/how-trumps-approach-middle-east-ignores-past-future-and-human-condition
   INFO:root:rank=6 pagerank=4.0936e-03 url=www.lawfareblog.com/why-trump-cant-buy-greenland
   INFO:root:rank=7 pagerank=3.7592e-03 url=www.lawfareblog.com/oral-argument-summary-qassim-v-trump
   INFO:root:rank=8 pagerank=3.4510e-03 url=www.lawfareblog.com/dc-circuit-court-denies-trump-rehearing-mazars-case
   INFO:root:rank=9 pagerank=3.4486e-03 url=www.lawfareblog.com/second-circuit-rules-mazars-must-hand-over-trump-tax-returns-new-york-prosecutors

   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='iran'
   INFO:root:rank=0 pagerank=4.5748e-03 url=www.lawfareblog.com/praise-presidents-iran-tweets
   INFO:root:rank=1 pagerank=4.4176e-03 url=www.lawfareblog.com/how-us-iran-tensions-could-disrupt-iraqs-fragile-peace
   INFO:root:rank=2 pagerank=2.6929e-03 url=www.lawfareblog.com/cyber-command-operational-update-clarifying-june-2019-iran-operation
   INFO:root:rank=3 pagerank=1.9392e-03 url=www.lawfareblog.com/aborted-iran-strike-fine-line-between-necessity-and-revenge
   INFO:root:rank=4 pagerank=1.5453e-03 url=www.lawfareblog.com/parsing-state-departments-letter-use-force-against-iran
   INFO:root:rank=5 pagerank=1.5358e-03 url=www.lawfareblog.com/iranian-hostage-crisis-and-its-effect-american-politics
   INFO:root:rank=6 pagerank=1.5258e-03 url=www.lawfareblog.com/announcing-united-states-and-use-force-against-iran-new-lawfare-e-book
   INFO:root:rank=7 pagerank=1.4222e-03 url=www.lawfareblog.com/us-names-iranian-revolutionary-guard-terrorist-organization-and-sanctions-international-criminal
   INFO:root:rank=8 pagerank=1.1788e-03 url=www.lawfareblog.com/iran-shoots-down-us-drone-domestic-and-international-legal-implications
   INFO:root:rank=9 pagerank=1.1463e-03 url=www.lawfareblog.com/israel-iran-syria-clash-and-law-use-force
   ```

   Task 1, part 3:
   ```
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz
   INFO:root:rank=0 pagerank=2.8741e-01 url=www.lawfareblog.com/about-lawfare-brief-history-term-and-site
   INFO:root:rank=1 pagerank=2.8741e-01 url=www.lawfareblog.com/lawfare-job-board
   INFO:root:rank=2 pagerank=2.8741e-01 url=www.lawfareblog.com/litigation-documents-resources-related-travel-ban
   INFO:root:rank=3 pagerank=2.8741e-01 url=www.lawfareblog.com/subscribe-lawfare
   INFO:root:rank=4 pagerank=2.8741e-01 url=www.lawfareblog.com/our-comments-policy
   INFO:root:rank=5 pagerank=2.8741e-01 url=www.lawfareblog.com/upcoming-events
   INFO:root:rank=6 pagerank=2.8741e-01 url=www.lawfareblog.com/support-lawfare
   INFO:root:rank=7 pagerank=2.8741e-01 url=www.lawfareblog.com/snowden-revelations
   INFO:root:rank=8 pagerank=2.8741e-01 url=www.lawfareblog.com/topics
   INFO:root:rank=9 pagerank=2.8741e-01 url=www.lawfareblog.com/documents-related-mueller-investigation

   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2
   INFO:root:rank=0 pagerank=3.5221e-01 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
   INFO:root:rank=1 pagerank=2.9850e-01 url=www.lawfareblog.com/livestream-nov-21-impeachment-hearings-0
   INFO:root:rank=2 pagerank=2.9371e-01 url=www.lawfareblog.com/opening-statement-david-holmes
   INFO:root:rank=3 pagerank=1.5110e-01 url=www.lawfareblog.com/lawfare-podcast-ben-nimmo-whack-mole-game-disinformation
   INFO:root:rank=4 pagerank=1.5002e-01 url=www.lawfareblog.com/lawfare-podcast-week-was-impeachment
   INFO:root:rank=5 pagerank=1.4828e-01 url=www.lawfareblog.com/todays-headlines-and-commentary-1963
   INFO:root:rank=6 pagerank=1.4828e-01 url=www.lawfareblog.com/todays-headlines-and-commentary-1964
   INFO:root:rank=7 pagerank=1.4690e-01 url=www.lawfareblog.com/todays-headlines-and-commentary-1962
   INFO:root:rank=8 pagerank=1.4305e-01 url=www.lawfareblog.com/cyberlaw-podcast-mistrusting-google
   INFO:root:rank=9 pagerank=1.4189e-01 url=www.lawfareblog.com/lawfare-podcast-bonus-edition-gordon-sondland-vs-committee-no-bull
   ```

   Task 1, part 4:
   ```
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose 
   DEBUG:root:computing indices
   DEBUG:root:computing values
   DEBUG:root:i=0 residual=1.3793749809265137
   DEBUG:root:i=1 residual=0.11642683297395706
   DEBUG:root:i=2 residual=0.07496178895235062
   DEBUG:root:i=3 residual=0.031702104955911636
   DEBUG:root:i=4 residual=0.0174466110765934
   DEBUG:root:i=5 residual=0.008526231162250042
   DEBUG:root:i=6 residual=0.00444182800129056
   DEBUG:root:i=7 residual=0.0022433267440646887
   DEBUG:root:i=8 residual=0.001149666146375239
   DEBUG:root:i=9 residual=0.0005811726441606879
   DEBUG:root:i=10 residual=0.00029266104684211314
   DEBUG:root:i=11 residual=0.00014553753135260195
   DEBUG:root:i=12 residual=7.151532918214798e-05
   DEBUG:root:i=13 residual=3.476878555375151e-05
   DEBUG:root:i=14 residual=1.5952729881973937e-05
   DEBUG:root:i=15 residual=6.454707545344718e-06
   DEBUG:root:i=16 residual=2.470087110850727e-06
   DEBUG:root:i=17 residual=8.236708595177333e-07
   INFO:root:rank=0 pagerank=2.8741e-01 url=www.lawfareblog.com/about-lawfare-brief-history-term-and-site
   INFO:root:rank=1 pagerank=2.8741e-01 url=www.lawfareblog.com/lawfare-job-board
   INFO:root:rank=2 pagerank=2.8741e-01 url=www.lawfareblog.com/litigation-documents-resources-related-travel-ban
   INFO:root:rank=3 pagerank=2.8741e-01 url=www.lawfareblog.com/subscribe-lawfare
   INFO:root:rank=4 pagerank=2.8741e-01 url=www.lawfareblog.com/our-comments-policy
   INFO:root:rank=5 pagerank=2.8741e-01 url=www.lawfareblog.com/upcoming-events
   INFO:root:rank=6 pagerank=2.8741e-01 url=www.lawfareblog.com/support-lawfare
   INFO:root:rank=7 pagerank=2.8741e-01 url=www.lawfareblog.com/snowden-revelations
   INFO:root:rank=8 pagerank=2.8741e-01 url=www.lawfareblog.com/topics
   INFO:root:rank=9 pagerank=2.8741e-01 url=www.lawfareblog.com/documents-related-mueller-investigation

   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --alpha=0.99999
   DEBUG:root:computing indices
   DEBUG:root:computing values
   DEBUG:root:i=0 residual=1.384641170501709
   DEBUG:root:i=1 residual=0.07088145613670349
   DEBUG:root:i=2 residual=0.01882273517549038
   DEBUG:root:i=3 residual=0.006958308629691601
   DEBUG:root:i=4 residual=0.0027358275838196278
   DEBUG:root:i=5 residual=0.0010345610789954662
   DEBUG:root:i=6 residual=0.0003774643409997225
   DEBUG:root:i=7 residual=0.0001353343395749107
   DEBUG:root:i=8 residual=4.822430855710991e-05
   DEBUG:root:i=9 residual=1.717166742309928e-05
   DEBUG:root:i=10 residual=6.1166115301602986e-06
   DEBUG:root:i=11 residual=2.1727698822360253e-06
   DEBUG:root:i=12 residual=7.75930004692782e-07
   INFO:root:rank=0 pagerank=2.8859e-01 url=www.lawfareblog.com/about-lawfare-brief-history-term-and-site
   INFO:root:rank=1 pagerank=2.8859e-01 url=www.lawfareblog.com/lawfare-job-board
   INFO:root:rank=2 pagerank=2.8859e-01 url=www.lawfareblog.com/litigation-documents-resources-related-travel-ban
   INFO:root:rank=3 pagerank=2.8859e-01 url=www.lawfareblog.com/subscribe-lawfare
   INFO:root:rank=4 pagerank=2.8859e-01 url=www.lawfareblog.com/our-comments-policy
   INFO:root:rank=5 pagerank=2.8859e-01 url=www.lawfareblog.com/upcoming-events
   INFO:root:rank=6 pagerank=2.8859e-01 url=www.lawfareblog.com/support-lawfare
   INFO:root:rank=7 pagerank=2.8859e-01 url=www.lawfareblog.com/snowden-revelations
   INFO:root:rank=8 pagerank=2.8859e-01 url=www.lawfareblog.com/topics
   INFO:root:rank=9 pagerank=2.8859e-01 url=www.lawfareblog.com/documents-related-mueller-investigation

   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --filter_ratio=0.2
   DEBUG:root:computing indices
   DEBUG:root:computing values
   DEBUG:root:i=0 residual=1.2714414596557617
   DEBUG:root:i=1 residual=0.5307188630104065
   DEBUG:root:i=2 residual=0.13826799392700195
   DEBUG:root:i=3 residual=0.07753033190965652
   DEBUG:root:i=4 residual=0.025020388886332512
   DEBUG:root:i=5 residual=0.010673251003026962
   DEBUG:root:i=6 residual=0.005278122611343861
   DEBUG:root:i=7 residual=0.0024619095493108034
   DEBUG:root:i=8 residual=0.0011817105114459991
   DEBUG:root:i=9 residual=0.0005855977651663125
   DEBUG:root:i=10 residual=0.0003050161467399448
   DEBUG:root:i=11 residual=0.00016693375073373318
   DEBUG:root:i=12 residual=9.558071906212717e-05
   DEBUG:root:i=13 residual=5.665007120114751e-05
   DEBUG:root:i=14 residual=3.4315846278332174e-05
   DEBUG:root:i=15 residual=2.0995004888391122e-05
   DEBUG:root:i=16 residual=1.2913144928461406e-05
   DEBUG:root:i=17 residual=7.92059836385306e-06
   DEBUG:root:i=18 residual=4.8281531235261355e-06
   DEBUG:root:i=19 residual=2.93107427751238e-06
   DEBUG:root:i=20 residual=1.7644197214394808e-06
   DEBUG:root:i=21 residual=1.0617327461659443e-06
   DEBUG:root:i=22 residual=6.350795160869893e-07
   INFO:root:rank=0 pagerank=3.5221e-01 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
   INFO:root:rank=1 pagerank=2.9850e-01 url=www.lawfareblog.com/livestream-nov-21-impeachment-hearings-0
   INFO:root:rank=2 pagerank=2.9371e-01 url=www.lawfareblog.com/opening-statement-david-holmes
   INFO:root:rank=3 pagerank=1.5110e-01 url=www.lawfareblog.com/lawfare-podcast-ben-nimmo-whack-mole-game-disinformation
   INFO:root:rank=4 pagerank=1.5002e-01 url=www.lawfareblog.com/lawfare-podcast-week-was-impeachment
   INFO:root:rank=5 pagerank=1.4828e-01 url=www.lawfareblog.com/todays-headlines-and-commentary-1963
   INFO:root:rank=6 pagerank=1.4828e-01 url=www.lawfareblog.com/todays-headlines-and-commentary-1964
   INFO:root:rank=7 pagerank=1.4690e-01 url=www.lawfareblog.com/todays-headlines-and-commentary-1962
   INFO:root:rank=8 pagerank=1.4305e-01 url=www.lawfareblog.com/cyberlaw-podcast-mistrusting-google
   INFO:root:rank=9 pagerank=1.4189e-01 url=www.lawfareblog.com/lawfare-podcast-bonus-edition-gordon-sondland-vs-committee-no-bull

   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --filter_ratio=0.2 --alpha=0.99999
   DEBUG:root:computing indices
   DEBUG:root:computing values
   DEBUG:root:i=0 residual=1.2932230234146118
   DEBUG:root:i=1 residual=0.6075857877731323
   DEBUG:root:i=2 residual=0.3771006166934967
   DEBUG:root:i=3 residual=0.20986923575401306
   DEBUG:root:i=4 residual=0.136985182762146
   DEBUG:root:i=5 residual=0.10712184756994247
   DEBUG:root:i=6 residual=0.09208471328020096
   DEBUG:root:i=7 residual=0.08161521703004837
   DEBUG:root:i=8 residual=0.07276003807783127
   DEBUG:root:i=9 residual=0.06502140313386917
   DEBUG:root:i=10 residual=0.058597762137651443
   DEBUG:root:i=11 residual=0.05381738394498825
   DEBUG:root:i=12 residual=0.05093031004071236
   DEBUG:root:i=13 residual=0.049981724470853806
   DEBUG:root:i=14 residual=0.05074530467391014
   DEBUG:root:i=15 residual=0.052765220403671265
   DEBUG:root:i=16 residual=0.055477265268564224
   DEBUG:root:i=17 residual=0.05832662433385849
   DEBUG:root:i=18 residual=0.060838326811790466
   DEBUG:root:i=19 residual=0.0626516342163086
   DEBUG:root:i=20 residual=0.06353529542684555
   DEBUG:root:i=21 residual=0.06339021027088165
   DEBUG:root:i=22 residual=0.06223801523447037
   DEBUG:root:i=23 residual=0.06019633635878563
   DEBUG:root:i=24 residual=0.05744423344731331
   DEBUG:root:i=25 residual=0.054186854511499405
   DEBUG:root:i=26 residual=0.05062471702694893
   DEBUG:root:i=27 residual=0.046933386474847794
   DEBUG:root:i=28 residual=0.043253093957901
   DEBUG:root:i=29 residual=0.039687082171440125
   DEBUG:root:i=30 residual=0.0363045260310173
   DEBUG:root:i=31 residual=0.03314671292901039
   DEBUG:root:i=32 residual=0.030233418568968773
   DEBUG:root:i=33 residual=0.02756926603615284
   DEBUG:root:i=34 residual=0.025148065760731697
   DEBUG:root:i=35 residual=0.022957829758524895
   DEBUG:root:i=36 residual=0.020982110872864723
   DEBUG:root:i=37 residual=0.019203398376703262
   DEBUG:root:i=38 residual=0.017603568732738495
   DEBUG:root:i=39 residual=0.0161651112139225
   DEBUG:root:i=40 residual=0.01487151812762022
   DEBUG:root:i=41 residual=0.013707430101931095
   DEBUG:root:i=42 residual=0.012658888474106789
   DEBUG:root:i=43 residual=0.01171331200748682
   DEBUG:root:i=44 residual=0.010859549045562744
   DEBUG:root:i=45 residual=0.010087382048368454
   DEBUG:root:i=46 residual=0.009388020262122154
   DEBUG:root:i=47 residual=0.00875353068113327
   DEBUG:root:i=48 residual=0.008176857605576515
   DEBUG:root:i=49 residual=0.007651915308088064
   DEBUG:root:i=50 residual=0.007173224352300167
   DEBUG:root:i=51 residual=0.006735950242727995
   DEBUG:root:i=52 residual=0.006335797253996134
   DEBUG:root:i=53 residual=0.005968950688838959
   DEBUG:root:i=54 residual=0.005632137414067984
   DEBUG:root:i=55 residual=0.0053223734721541405
   DEBUG:root:i=56 residual=0.0050370036624372005
   DEBUG:root:i=57 residual=0.0047737006098032
   DEBUG:root:i=58 residual=0.004530338104814291
   DEBUG:root:i=59 residual=0.004305060487240553
   DEBUG:root:i=60 residual=0.004096208605915308
   DEBUG:root:i=61 residual=0.0039023091085255146
   DEBUG:root:i=62 residual=0.003722006920725107
   DEBUG:root:i=63 residual=0.0035541034303605556
   DEBUG:root:i=64 residual=0.0033975602127611637
   DEBUG:root:i=65 residual=0.0032513695769011974
   DEBUG:root:i=66 residual=0.003114705439656973
   DEBUG:root:i=67 residual=0.0029867393895983696
   DEBUG:root:i=68 residual=0.002866796450689435
   DEBUG:root:i=69 residual=0.0027541983872652054
   DEBUG:root:i=70 residual=0.0026483903639018536
   DEBUG:root:i=71 residual=0.0025488503742963076
   DEBUG:root:i=72 residual=0.00245510321110487
   DEBUG:root:i=73 residual=0.0023666671477258205
   DEBUG:root:i=74 residual=0.0022832010872662067
   DEBUG:root:i=75 residual=0.0022043169010430574
   DEBUG:root:i=76 residual=0.002129694912582636
   DEBUG:root:i=77 residual=0.002059011720120907
   DEBUG:root:i=78 residual=0.0019920181948691607
   DEBUG:root:i=79 residual=0.0019284730078652501
   DEBUG:root:i=80 residual=0.0018680969951674342
   DEBUG:root:i=81 residual=0.0018107080832123756
   DEBUG:root:i=82 residual=0.0017560927662998438
   DEBUG:root:i=83 residual=0.0017041193787008524
   DEBUG:root:i=84 residual=0.0016545511316508055
   DEBUG:root:i=85 residual=0.0016072704456746578
   DEBUG:root:i=86 residual=0.0015621442580595613
   DEBUG:root:i=87 residual=0.0015189982950687408
   DEBUG:root:i=88 residual=0.0014777646865695715
   DEBUG:root:i=89 residual=0.001438300358131528
   DEBUG:root:i=90 residual=0.0014005283592268825
   DEBUG:root:i=91 residual=0.0013643096899613738
   DEBUG:root:i=92 residual=0.0013295902172103524
   DEBUG:root:i=93 residual=0.0012962680775672197
   DEBUG:root:i=94 residual=0.00126426643691957
   DEBUG:root:i=95 residual=0.0012335155624896288
   DEBUG:root:i=96 residual=0.0012039435096085072
   DEBUG:root:i=97 residual=0.0011755152372643352
   DEBUG:root:i=98 residual=0.0011481251567602158
   DEBUG:root:i=99 residual=0.0011217388091608882
   DEBUG:root:i=100 residual=0.0010963198728859425
   DEBUG:root:i=101 residual=0.0010718059493228793
   DEBUG:root:i=102 residual=0.001048146397806704
   DEBUG:root:i=103 residual=0.0010253068758174777
   DEBUG:root:i=104 residual=0.0010032416321337223
   DEBUG:root:i=105 residual=0.0009819157421588898
   DEBUG:root:i=106 residual=0.0009613021393306553
   DEBUG:root:i=107 residual=0.0009413553634658456
   DEBUG:root:i=108 residual=0.0009220482315868139
   DEBUG:root:i=109 residual=0.0009033613023348153
   DEBUG:root:i=110 residual=0.000885249930433929
   DEBUG:root:i=111 residual=0.0008676886791363358
   DEBUG:root:i=112 residual=0.0008506776066496968
   DEBUG:root:i=113 residual=0.0008341650827787817
   DEBUG:root:i=114 residual=0.0008181394077837467
   DEBUG:root:i=115 residual=0.0008025867864489555
   DEBUG:root:i=116 residual=0.0007874760194681585
   DEBUG:root:i=117 residual=0.0007727991323918104
   DEBUG:root:i=118 residual=0.000758520734962076
   DEBUG:root:i=119 residual=0.0007446478120982647
   DEBUG:root:i=120 residual=0.000731149862986058
   DEBUG:root:i=121 residual=0.0007180118118412793
   DEBUG:root:i=122 residual=0.0007052180008031428
   DEBUG:root:i=123 residual=0.0006927722715772688
   DEBUG:root:i=124 residual=0.0006806409219279885
   DEBUG:root:i=125 residual=0.0006688254652544856
   DEBUG:root:i=126 residual=0.0006572984857484698
   DEBUG:root:i=127 residual=0.0006460747099481523
   DEBUG:root:i=128 residual=0.0006351175252348185
   DEBUG:root:i=129 residual=0.0006244322867132723
   DEBUG:root:i=130 residual=0.0006140071200206876
   DEBUG:root:i=131 residual=0.0006038236315362155
   DEBUG:root:i=132 residual=0.000593891367316246
   DEBUG:root:i=133 residual=0.0005841813399456441
   DEBUG:root:i=134 residual=0.0005746985552832484
   DEBUG:root:i=135 residual=0.0005654277047142386
   DEBUG:root:i=136 residual=0.0005563714657910168
   DEBUG:root:i=137 residual=0.0005475187790580094
   DEBUG:root:i=138 residual=0.0005388556746765971
   DEBUG:root:i=139 residual=0.0005303916404955089
   DEBUG:root:i=140 residual=0.0005220999009907246
   DEBUG:root:i=141 residual=0.0005139895365573466
   DEBUG:root:i=142 residual=0.0005060540279373527
   DEBUG:root:i=143 residual=0.0004982837708666921
   DEBUG:root:i=144 residual=0.0004906749818474054
   DEBUG:root:i=145 residual=0.00048321913345716894
   DEBUG:root:i=146 residual=0.00047592463670298457
   DEBUG:root:i=147 residual=0.0004687742330133915
   DEBUG:root:i=148 residual=0.000461763673229143
   DEBUG:root:i=149 residual=0.0004548995057120919
   DEBUG:root:i=150 residual=0.00044816816807724535
   DEBUG:root:i=151 residual=0.00044156520743854344
   DEBUG:root:i=152 residual=0.0004350940871518105
   DEBUG:root:i=153 residual=0.0004287451156415045
   DEBUG:root:i=154 residual=0.0004225196607876569
   DEBUG:root:i=155 residual=0.0004164061974734068
   DEBUG:root:i=156 residual=0.0004104151448700577
   DEBUG:root:i=157 residual=0.00040453491965308785
   DEBUG:root:i=158 residual=0.0003987560630775988
   DEBUG:root:i=159 residual=0.0003930960956495255
   DEBUG:root:i=160 residual=0.0003875300462823361
   DEBUG:root:i=161 residual=0.0003820627462118864
   DEBUG:root:i=162 residual=0.0003766979498323053
   DEBUG:root:i=163 residual=0.000371425470802933
   DEBUG:root:i=164 residual=0.00036625517532229424
   DEBUG:root:i=165 residual=0.0003611660504247993
   DEBUG:root:i=166 residual=0.0003561688936315477
   DEBUG:root:i=167 residual=0.00035125776776112616
   DEBUG:root:i=168 residual=0.0003464318870101124
   DEBUG:root:i=169 residual=0.0003416895342525095
   DEBUG:root:i=170 residual=0.0003370266640558839
   DEBUG:root:i=171 residual=0.0003324415010865778
   DEBUG:root:i=172 residual=0.00032793093123473227
   DEBUG:root:i=173 residual=0.0003235002513974905
   DEBUG:root:i=174 residual=0.0003191466676071286
   DEBUG:root:i=175 residual=0.0003148525720462203
   DEBUG:root:i=176 residual=0.0003106422955170274
   DEBUG:root:i=177 residual=0.00030649869586341083
   DEBUG:root:i=178 residual=0.00030241336207836866
   DEBUG:root:i=179 residual=0.0002984006714541465
   DEBUG:root:i=180 residual=0.000294452445814386
   DEBUG:root:i=181 residual=0.00029056804487481713
   DEBUG:root:i=182 residual=0.0002867468574550003
   DEBUG:root:i=183 residual=0.00028298282995820045
   DEBUG:root:i=184 residual=0.0002792781451717019
   DEBUG:root:i=185 residual=0.0002756331523414701
   DEBUG:root:i=186 residual=0.000272043194854632
   DEBUG:root:i=187 residual=0.00026850850554183125
   DEBUG:root:i=188 residual=0.0002650298993103206
   DEBUG:root:i=189 residual=0.0002616051060613245
   DEBUG:root:i=190 residual=0.00025823398027569056
   DEBUG:root:i=191 residual=0.0002549118362367153
   DEBUG:root:i=192 residual=0.00025164015823975205
   DEBUG:root:i=193 residual=0.0002484181022737175
   DEBUG:root:i=194 residual=0.0002452441258355975
   DEBUG:root:i=195 residual=0.00024211977142840624
   DEBUG:root:i=196 residual=0.00023904131376184523
   DEBUG:root:i=197 residual=0.0002360078360652551
   DEBUG:root:i=198 residual=0.0002330178249394521
   DEBUG:root:i=199 residual=0.00023007430718280375
   DEBUG:root:i=200 residual=0.0002271700941491872
   DEBUG:root:i=201 residual=0.00022431198158301413
   DEBUG:root:i=202 residual=0.00022149397409521043
   DEBUG:root:i=203 residual=0.0002187185309594497
   DEBUG:root:i=204 residual=0.0002159817231586203
   DEBUG:root:i=205 residual=0.00021328552975319326
   DEBUG:root:i=206 residual=0.00021062734595034271
   DEBUG:root:i=207 residual=0.0002080052945530042
   DEBUG:root:i=208 residual=0.000205423406441696
   DEBUG:root:i=209 residual=0.00020287717052269727
   DEBUG:root:i=210 residual=0.00020036619389429688
   DEBUG:root:i=211 residual=0.0001978888176381588
   DEBUG:root:i=212 residual=0.00019544785027392209
   DEBUG:root:i=213 residual=0.0001930429571075365
   DEBUG:root:i=214 residual=0.00019067039829678833
   DEBUG:root:i=215 residual=0.00018832896603271365
   DEBUG:root:i=216 residual=0.00018602180352900177
   DEBUG:root:i=217 residual=0.00018374857609160244
   DEBUG:root:i=218 residual=0.00018150336109101772
   DEBUG:root:i=219 residual=0.000179292619577609
   DEBUG:root:i=220 residual=0.00017710949759930372
   DEBUG:root:i=221 residual=0.00017495499923825264
   DEBUG:root:i=222 residual=0.00017283267516177148
   DEBUG:root:i=223 residual=0.00017073866911232471
   DEBUG:root:i=224 residual=0.00016867309750523418
   DEBUG:root:i=225 residual=0.00016663470887579024
   DEBUG:root:i=226 residual=0.00016462482744827867
   DEBUG:root:i=227 residual=0.00016263996076304466
   DEBUG:root:i=228 residual=0.00016068460536189377
   DEBUG:root:i=229 residual=0.00015875065582804382
   DEBUG:root:i=230 residual=0.00015684649406466633
   DEBUG:root:i=231 residual=0.00015496730338782072
   DEBUG:root:i=232 residual=0.00015311302558984607
   DEBUG:root:i=233 residual=0.00015128194354474545
   DEBUG:root:i=234 residual=0.00014947673480492085
   DEBUG:root:i=235 residual=0.0001476937613915652
   DEBUG:root:i=236 residual=0.0001459327613702044
   DEBUG:root:i=237 residual=0.00014420018123928457
   DEBUG:root:i=238 residual=0.00014248375373426825
   DEBUG:root:i=239 residual=0.0001407929084962234
   DEBUG:root:i=240 residual=0.0001391263649566099
   DEBUG:root:i=241 residual=0.00013747747289016843
   DEBUG:root:i=242 residual=0.00013585244596470147
   DEBUG:root:i=243 residual=0.00013424722419586033
   DEBUG:root:i=244 residual=0.00013266433961689472
   DEBUG:root:i=245 residual=0.0001310998050030321
   DEBUG:root:i=246 residual=0.000129555759485811
   DEBUG:root:i=247 residual=0.00012803317804355174
   DEBUG:root:i=248 residual=0.0001265301398234442
   DEBUG:root:i=249 residual=0.0001250460627488792
   DEBUG:root:i=250 residual=0.00012357976811472327
   DEBUG:root:i=251 residual=0.00012213319132570177
   DEBUG:root:i=252 residual=0.00012070561206201091
   DEBUG:root:i=253 residual=0.00011929199536098167
   DEBUG:root:i=254 residual=0.00011790091230068356
   DEBUG:root:i=255 residual=0.00011652648390736431
   DEBUG:root:i=256 residual=0.00011516718222992495
   DEBUG:root:i=257 residual=0.00011382696538930759
   DEBUG:root:i=258 residual=0.00011250260286033154
   DEBUG:root:i=259 residual=0.00011119488772237673
   DEBUG:root:i=260 residual=0.00010990338341798633
   DEBUG:root:i=261 residual=0.00010862813360290602
   DEBUG:root:i=262 residual=0.00010737044794950634
   DEBUG:root:i=263 residual=0.00010612676123855636
   DEBUG:root:i=264 residual=0.00010489610576769337
   DEBUG:root:i=265 residual=0.00010368337098043412
   DEBUG:root:i=266 residual=0.00010248677426716313
   DEBUG:root:i=267 residual=0.00010130587907042354
   DEBUG:root:i=268 residual=0.00010013637802330777
   DEBUG:root:i=269 residual=9.898117423290387e-05
   DEBUG:root:i=270 residual=9.784391295397654e-05
   DEBUG:root:i=271 residual=9.671717998571694e-05
   DEBUG:root:i=272 residual=9.56062285695225e-05
   DEBUG:root:i=273 residual=9.450753714190796e-05
   DEBUG:root:i=274 residual=9.342295379610732e-05
   DEBUG:root:i=275 residual=9.235229663318023e-05
   DEBUG:root:i=276 residual=9.129472164204344e-05
   DEBUG:root:i=277 residual=9.024869359564036e-05
   DEBUG:root:i=278 residual=8.921591506805271e-05
   DEBUG:root:i=279 residual=8.819683716865256e-05
   DEBUG:root:i=280 residual=8.719060861039907e-05
   DEBUG:root:i=281 residual=8.619410073151812e-05
   DEBUG:root:i=282 residual=8.521108975401148e-05
   DEBUG:root:i=283 residual=8.423986582783982e-05
   DEBUG:root:i=284 residual=8.327847899636254e-05
   DEBUG:root:i=285 residual=8.233125845436007e-05
   DEBUG:root:i=286 residual=8.13963488326408e-05
   DEBUG:root:i=287 residual=8.047077426454052e-05
   DEBUG:root:i=288 residual=7.955488399602473e-05
   DEBUG:root:i=289 residual=7.865230145398527e-05
   DEBUG:root:i=290 residual=7.77601744630374e-05
   DEBUG:root:i=291 residual=7.687696779612452e-05
   DEBUG:root:i=292 residual=7.600684330100194e-05
   DEBUG:root:i=293 residual=7.514697063015774e-05
   DEBUG:root:i=294 residual=7.429596007568762e-05
   DEBUG:root:i=295 residual=7.345532503677532e-05
   DEBUG:root:i=296 residual=7.262413419084623e-05
   DEBUG:root:i=297 residual=7.180388638516888e-05
   DEBUG:root:i=298 residual=7.099306822055951e-05
   DEBUG:root:i=299 residual=7.019169424893335e-05
   DEBUG:root:i=300 residual=6.939988088561222e-05
   DEBUG:root:i=301 residual=6.861711153760552e-05
   DEBUG:root:i=302 residual=6.784303695894778e-05
   DEBUG:root:i=303 residual=6.707950524287298e-05
   DEBUG:root:i=304 residual=6.632642907788977e-05
   DEBUG:root:i=305 residual=6.558003224199638e-05
   DEBUG:root:i=306 residual=6.48415443720296e-05
   DEBUG:root:i=307 residual=6.411397771444172e-05
   DEBUG:root:i=308 residual=6.339476385619491e-05
   DEBUG:root:i=309 residual=6.268240395002067e-05
   DEBUG:root:i=310 residual=6.197744369274005e-05
   DEBUG:root:i=311 residual=6.128294626250863e-05
   DEBUG:root:i=312 residual=6.059931547497399e-05
   DEBUG:root:i=313 residual=5.9916426835116e-05
   DEBUG:root:i=314 residual=5.924655852140859e-05
   DEBUG:root:i=315 residual=5.8584158978192136e-05
   DEBUG:root:i=316 residual=5.79275656491518e-05
   DEBUG:root:i=317 residual=5.7281169574707747e-05
   DEBUG:root:i=318 residual=5.6640397815499455e-05
   DEBUG:root:i=319 residual=5.600846270681359e-05
   DEBUG:root:i=320 residual=5.5382042773999274e-05
   DEBUG:root:i=321 residual=5.4764932428952307e-05
   DEBUG:root:i=322 residual=5.4153129894984886e-05
   DEBUG:root:i=323 residual=5.35483741259668e-05
   DEBUG:root:i=324 residual=5.2952993428334594e-05
   DEBUG:root:i=325 residual=5.236219658399932e-05
   DEBUG:root:i=326 residual=5.1778682973235846e-05
   DEBUG:root:i=327 residual=5.1200455345679075e-05
   DEBUG:root:i=328 residual=5.063166099716909e-05
   DEBUG:root:i=329 residual=5.0069629651261494e-05
   DEBUG:root:i=330 residual=4.951220762450248e-05
   DEBUG:root:i=331 residual=4.896186510450207e-05
   DEBUG:root:i=332 residual=4.841841655434109e-05
   DEBUG:root:i=333 residual=4.787995931110345e-05
   DEBUG:root:i=334 residual=4.734910180559382e-05
   DEBUG:root:i=335 residual=4.6823941374896094e-05
   DEBUG:root:i=336 residual=4.6304328861879185e-05
   DEBUG:root:i=337 residual=4.578995140036568e-05
   DEBUG:root:i=338 residual=4.528334102360532e-05
   DEBUG:root:i=339 residual=4.478088885662146e-05
   DEBUG:root:i=340 residual=4.428426473168656e-05
   DEBUG:root:i=341 residual=4.379407619126141e-05
   DEBUG:root:i=342 residual=4.3309497414156795e-05
   DEBUG:root:i=343 residual=4.2830575694097206e-05
   DEBUG:root:i=344 residual=4.235606320435181e-05
   DEBUG:root:i=345 residual=4.1889736166922376e-05
   DEBUG:root:i=346 residual=4.142502439208329e-05
   DEBUG:root:i=347 residual=4.096960765309632e-05
   DEBUG:root:i=348 residual=4.051520227221772e-05
   DEBUG:root:i=349 residual=4.006862945971079e-05
   DEBUG:root:i=350 residual=3.9625207136850804e-05
   DEBUG:root:i=351 residual=3.918903530575335e-05
   DEBUG:root:i=352 residual=3.87553773180116e-05
   DEBUG:root:i=353 residual=3.832925358437933e-05
   DEBUG:root:i=354 residual=3.790552727878094e-05
   DEBUG:root:i=355 residual=3.748800008906983e-05
   DEBUG:root:i=356 residual=3.7075667933095247e-05
   DEBUG:root:i=357 residual=3.666572956717573e-05
   DEBUG:root:i=358 residual=3.626284160418436e-05
   DEBUG:root:i=359 residual=3.586271850508638e-05
   DEBUG:root:i=360 residual=3.546801963238977e-05
   DEBUG:root:i=361 residual=3.507999281282537e-05
   DEBUG:root:i=362 residual=3.469291914370842e-05
   DEBUG:root:i=363 residual=3.4312404750380665e-05
   DEBUG:root:i=364 residual=3.393467341084033e-05
   DEBUG:root:i=365 residual=3.3562489988980815e-05
   DEBUG:root:i=366 residual=3.319194365758449e-05
   DEBUG:root:i=367 residual=3.282821853645146e-05
   DEBUG:root:i=368 residual=3.246620326535776e-05
   DEBUG:root:i=369 residual=3.210968861822039e-05
   DEBUG:root:i=370 residual=3.175812162226066e-05
   DEBUG:root:i=371 residual=3.141037086606957e-05
   DEBUG:root:i=372 residual=3.1066218070918694e-05
   DEBUG:root:i=373 residual=3.072417530347593e-05
   DEBUG:root:i=374 residual=3.0388117011170834e-05
   DEBUG:root:i=375 residual=3.005483085871674e-05
   DEBUG:root:i=376 residual=2.9726656066486612e-05
   DEBUG:root:i=377 residual=2.939938349300064e-05
   DEBUG:root:i=378 residual=2.907772250182461e-05
   DEBUG:root:i=379 residual=2.8758820917573757e-05
   DEBUG:root:i=380 residual=2.8443935661925934e-05
   DEBUG:root:i=381 residual=2.813250284816604e-05
   DEBUG:root:i=382 residual=2.7823578420793638e-05
   DEBUG:root:i=383 residual=2.752020191110205e-05
   DEBUG:root:i=384 residual=2.7220425181440078e-05
   DEBUG:root:i=385 residual=2.6921274184132926e-05
   DEBUG:root:i=386 residual=2.6627500119502656e-05
   DEBUG:root:i=387 residual=2.6335237635066733e-05
   DEBUG:root:i=388 residual=2.6049307052744552e-05
   DEBUG:root:i=389 residual=2.5762725272215903e-05
   DEBUG:root:i=390 residual=2.5481898774160072e-05
   DEBUG:root:i=391 residual=2.520315865695011e-05
   DEBUG:root:i=392 residual=2.4930137442424893e-05
   DEBUG:root:i=393 residual=2.4656259483890608e-05
   DEBUG:root:i=394 residual=2.4386965378653258e-05
   DEBUG:root:i=395 residual=2.412189860478975e-05
   DEBUG:root:i=396 residual=2.3858132408349775e-05
   DEBUG:root:i=397 residual=2.3597309336764738e-05
   DEBUG:root:i=398 residual=2.33416158152977e-05
   DEBUG:root:i=399 residual=2.308720286237076e-05
   DEBUG:root:i=400 residual=2.2834654373582453e-05
   DEBUG:root:i=401 residual=2.2585933038499206e-05
   DEBUG:root:i=402 residual=2.2338303097058088e-05
   DEBUG:root:i=403 residual=2.209583908552304e-05
   DEBUG:root:i=404 residual=2.185386802011635e-05
   DEBUG:root:i=405 residual=2.1616115191136487e-05
   DEBUG:root:i=406 residual=2.1381292754085734e-05
   DEBUG:root:i=407 residual=2.1147976440261118e-05
   DEBUG:root:i=408 residual=2.0917717847623862e-05
   DEBUG:root:i=409 residual=2.068974936264567e-05
   DEBUG:root:i=410 residual=2.0465990019147284e-05
   DEBUG:root:i=411 residual=2.024195418925956e-05
   DEBUG:root:i=412 residual=2.0021529053337872e-05
   DEBUG:root:i=413 residual=1.980529668799136e-05
   DEBUG:root:i=414 residual=1.9588223949540406e-05
   DEBUG:root:i=415 residual=1.9376777345314622e-05
   DEBUG:root:i=416 residual=1.9164246623404324e-05
   DEBUG:root:i=417 residual=1.895593413792085e-05
   DEBUG:root:i=418 residual=1.8750566596281715e-05
   DEBUG:root:i=419 residual=1.854817492130678e-05
   DEBUG:root:i=420 residual=1.8345257558394223e-05
   DEBUG:root:i=421 residual=1.814459392335266e-05
   DEBUG:root:i=422 residual=1.7949074390344322e-05
   DEBUG:root:i=423 residual=1.775298369466327e-05
   DEBUG:root:i=424 residual=1.755962148308754e-05
   DEBUG:root:i=425 residual=1.736764534143731e-05
   DEBUG:root:i=426 residual=1.717853592708707e-05
   DEBUG:root:i=427 residual=1.699142922007013e-05
   DEBUG:root:i=428 residual=1.6808206055429764e-05
   DEBUG:root:i=429 residual=1.66251375048887e-05
   DEBUG:root:i=430 residual=1.6445303117507137e-05
   DEBUG:root:i=431 residual=1.6265443264273927e-05
   DEBUG:root:i=432 residual=1.6089608834590763e-05
   DEBUG:root:i=433 residual=1.5914341929601505e-05
   DEBUG:root:i=434 residual=1.5742065443191677e-05
   DEBUG:root:i=435 residual=1.5570954928989522e-05
   DEBUG:root:i=436 residual=1.5400304619106464e-05
   DEBUG:root:i=437 residual=1.5233962585625704e-05
   DEBUG:root:i=438 residual=1.5069076653162483e-05
   DEBUG:root:i=439 residual=1.4906476280884817e-05
   DEBUG:root:i=440 residual=1.4744186046300456e-05
   DEBUG:root:i=441 residual=1.4584860764443874e-05
   DEBUG:root:i=442 residual=1.4427684618567582e-05
   DEBUG:root:i=443 residual=1.4271545296651311e-05
   DEBUG:root:i=444 residual=1.4116372767603025e-05
   DEBUG:root:i=445 residual=1.3961915101390332e-05
   DEBUG:root:i=446 residual=1.3810858035867568e-05
   DEBUG:root:i=447 residual=1.3661366210726555e-05
   DEBUG:root:i=448 residual=1.351276023342507e-05
   DEBUG:root:i=449 residual=1.3366858183871955e-05
   DEBUG:root:i=450 residual=1.322246953350259e-05
   DEBUG:root:i=451 residual=1.3080418284516782e-05
   DEBUG:root:i=452 residual=1.2938571671838872e-05
   DEBUG:root:i=453 residual=1.2799696378351655e-05
   DEBUG:root:i=454 residual=1.2660007996601053e-05
   DEBUG:root:i=455 residual=1.2522634278866462e-05
   DEBUG:root:i=456 residual=1.2387673450575676e-05
   DEBUG:root:i=457 residual=1.2253884051460773e-05
   DEBUG:root:i=458 residual=1.2121927284169942e-05
   DEBUG:root:i=459 residual=1.199076996272197e-05
   DEBUG:root:i=460 residual=1.1859587175422348e-05
   DEBUG:root:i=461 residual=1.173204873339273e-05
   DEBUG:root:i=462 residual=1.16042983790976e-05
   DEBUG:root:i=463 residual=1.148033425124595e-05
   DEBUG:root:i=464 residual=1.1355774404364638e-05
   DEBUG:root:i=465 residual=1.1232491488044616e-05
   DEBUG:root:i=466 residual=1.1111655112472363e-05
   DEBUG:root:i=467 residual=1.0991796443704516e-05
   DEBUG:root:i=468 residual=1.0872003258555196e-05
   DEBUG:root:i=469 residual=1.0754854883998632e-05
   DEBUG:root:i=470 residual=1.0638260391715448e-05
   DEBUG:root:i=471 residual=1.0523462151468266e-05
   DEBUG:root:i=472 residual=1.0410525646875612e-05
   DEBUG:root:i=473 residual=1.0298100278305355e-05
   DEBUG:root:i=474 residual=1.0186794497712981e-05
   DEBUG:root:i=475 residual=1.007677838060772e-05
   DEBUG:root:i=476 residual=9.967965524992906e-06
   DEBUG:root:i=477 residual=9.860815225692932e-06
   DEBUG:root:i=478 residual=9.754428901942447e-06
   DEBUG:root:i=479 residual=9.64868286246201e-06
   DEBUG:root:i=480 residual=9.543306987325195e-06
   DEBUG:root:i=481 residual=9.440853318665177e-06
   DEBUG:root:i=482 residual=9.338412382930983e-06
   DEBUG:root:i=483 residual=9.239657629223075e-06
   DEBUG:root:i=484 residual=9.138366294791922e-06
   DEBUG:root:i=485 residual=9.03927593753906e-06
   DEBUG:root:i=486 residual=8.944225555751473e-06
   DEBUG:root:i=487 residual=8.847111530485563e-06
   DEBUG:root:i=488 residual=8.75054502103012e-06
   DEBUG:root:i=489 residual=8.656805221107788e-06
   DEBUG:root:i=490 residual=8.562488801544532e-06
   DEBUG:root:i=491 residual=8.471256478514988e-06
   DEBUG:root:i=492 residual=8.379707651329227e-06
   DEBUG:root:i=493 residual=8.288349818030838e-06
   DEBUG:root:i=494 residual=8.197593160730321e-06
   DEBUG:root:i=495 residual=8.110108865366783e-06
   DEBUG:root:i=496 residual=8.023456757655367e-06
   DEBUG:root:i=497 residual=7.936191650514957e-06
   DEBUG:root:i=498 residual=7.85104748501908e-06
   DEBUG:root:i=499 residual=7.767027454974595e-06
   DEBUG:root:i=500 residual=7.682922841922846e-06
   DEBUG:root:i=501 residual=7.6004980655852705e-06
   DEBUG:root:i=502 residual=7.517128324252553e-06
   DEBUG:root:i=503 residual=7.4364165811857674e-06
   DEBUG:root:i=504 residual=7.35708408683422e-06
   DEBUG:root:i=505 residual=7.27762699170853e-06
   DEBUG:root:i=506 residual=7.198678758868482e-06
   DEBUG:root:i=507 residual=7.1218987613974605e-06
   DEBUG:root:i=508 residual=7.044588528515305e-06
   DEBUG:root:i=509 residual=6.969929472688818e-06
   DEBUG:root:i=510 residual=6.894251782796346e-06
   DEBUG:root:i=511 residual=6.818479050707538e-06
   DEBUG:root:i=512 residual=6.745521659468068e-06
   DEBUG:root:i=513 residual=6.6737998167809565e-06
   DEBUG:root:i=514 residual=6.600913820875576e-06
   DEBUG:root:i=515 residual=6.529871370730689e-06
   DEBUG:root:i=516 residual=6.45959244138794e-06
   DEBUG:root:i=517 residual=6.389544068952091e-06
   DEBUG:root:i=518 residual=6.320473858067999e-06
   DEBUG:root:i=519 residual=6.253620085772127e-06
   DEBUG:root:i=520 residual=6.1850505517213605e-06
   DEBUG:root:i=521 residual=6.11835139352479e-06
   DEBUG:root:i=522 residual=6.053927791072056e-06
   DEBUG:root:i=523 residual=5.986865289742127e-06
   DEBUG:root:i=524 residual=5.922540822211886e-06
   DEBUG:root:i=525 residual=5.860596502316184e-06
   DEBUG:root:i=526 residual=5.796125606138958e-06
   DEBUG:root:i=527 residual=5.733925718232058e-06
   DEBUG:root:i=528 residual=5.673293799191015e-06
   DEBUG:root:i=529 residual=5.611190772469854e-06
   DEBUG:root:i=530 residual=5.551747563004028e-06
   DEBUG:root:i=531 residual=5.490449439093936e-06
   DEBUG:root:i=532 residual=5.4322322284861e-06
   DEBUG:root:i=533 residual=5.373799467633944e-06
   DEBUG:root:i=534 residual=5.317796421877574e-06
   DEBUG:root:i=535 residual=5.258673354546772e-06
   DEBUG:root:i=536 residual=5.20121739100432e-06
   DEBUG:root:i=537 residual=5.144856913830154e-06
   DEBUG:root:i=538 residual=5.091716957394965e-06
   DEBUG:root:i=539 residual=5.0347071010037325e-06
   DEBUG:root:i=540 residual=4.98262170367525e-06
   DEBUG:root:i=541 residual=4.930591330776224e-06
   DEBUG:root:i=542 residual=4.876500042882981e-06
   DEBUG:root:i=543 residual=4.823349172511371e-06
   DEBUG:root:i=544 residual=4.770121904584812e-06
   DEBUG:root:i=545 residual=4.7173380153253675e-06
   DEBUG:root:i=546 residual=4.6688051043020096e-06
   DEBUG:root:i=547 residual=4.618846560333623e-06
   DEBUG:root:i=548 residual=4.569268639897928e-06
   DEBUG:root:i=549 residual=4.519813046499621e-06
   DEBUG:root:i=550 residual=4.470017756830202e-06
   DEBUG:root:i=551 residual=4.422920937940944e-06
   DEBUG:root:i=552 residual=4.3738655222114176e-06
   DEBUG:root:i=553 residual=4.326515409047715e-06
   DEBUG:root:i=554 residual=4.280885605112417e-06
   DEBUG:root:i=555 residual=4.2362712520116474e-06
   DEBUG:root:i=556 residual=4.19083198721637e-06
   DEBUG:root:i=557 residual=4.1451462493569124e-06
   DEBUG:root:i=558 residual=4.099468696949771e-06
   DEBUG:root:i=559 residual=4.056245870742714e-06
   DEBUG:root:i=560 residual=4.012710633105598e-06
   DEBUG:root:i=561 residual=3.969457793573383e-06
   DEBUG:root:i=562 residual=3.927509624190861e-06
   DEBUG:root:i=563 residual=3.885175374307437e-06
   DEBUG:root:i=564 residual=3.842262685793685e-06
   DEBUG:root:i=565 residual=3.8013258745195344e-06
   DEBUG:root:i=566 residual=3.760637810046319e-06
   DEBUG:root:i=567 residual=3.7211384551483206e-06
   DEBUG:root:i=568 residual=3.680431291286368e-06
   DEBUG:root:i=569 residual=3.640082013589563e-06
   DEBUG:root:i=570 residual=3.601710432121763e-06
   DEBUG:root:i=571 residual=3.5629079775389982e-06
   DEBUG:root:i=572 residual=3.5276771086500958e-06
   DEBUG:root:i=573 residual=3.486411287667579e-06
   DEBUG:root:i=574 residual=3.4475417578505585e-06
   DEBUG:root:i=575 residual=3.4123963814636227e-06
   DEBUG:root:i=576 residual=3.37684218720824e-06
   DEBUG:root:i=577 residual=3.3398553114238894e-06
   DEBUG:root:i=578 residual=3.3036239983630367e-06
   DEBUG:root:i=579 residual=3.267656893513049e-06
   DEBUG:root:i=580 residual=3.2329737678082893e-06
   DEBUG:root:i=581 residual=3.1981003303371836e-06
   DEBUG:root:i=582 residual=3.163713245157851e-06
   DEBUG:root:i=583 residual=3.128964863208239e-06
   DEBUG:root:i=584 residual=3.0967437396611786e-06
   DEBUG:root:i=585 residual=3.061941242776811e-06
   DEBUG:root:i=586 residual=3.0310636702779448e-06
   DEBUG:root:i=587 residual=2.998856189151411e-06
   DEBUG:root:i=588 residual=2.9643999823747436e-06
   DEBUG:root:i=589 residual=2.9342991183511913e-06
   DEBUG:root:i=590 residual=2.9015018299105577e-06
   DEBUG:root:i=591 residual=2.869493982871063e-06
   DEBUG:root:i=592 residual=2.841013156285044e-06
   DEBUG:root:i=593 residual=2.8089409624953987e-06
   DEBUG:root:i=594 residual=2.7805392619484337e-06
   DEBUG:root:i=595 residual=2.7483772555569885e-06
   DEBUG:root:i=596 residual=2.720392330957111e-06
   DEBUG:root:i=597 residual=2.691258714548894e-06
   DEBUG:root:i=598 residual=2.6613213321979856e-06
   DEBUG:root:i=599 residual=2.632400082802633e-06
   DEBUG:root:i=600 residual=2.607193891890347e-06
   DEBUG:root:i=601 residual=2.577515260782093e-06
   DEBUG:root:i=602 residual=2.547941448938218e-06
   DEBUG:root:i=603 residual=2.520800762795261e-06
   DEBUG:root:i=604 residual=2.4945795757957967e-06
   DEBUG:root:i=605 residual=2.4670689526828937e-06
   DEBUG:root:i=606 residual=2.4405683234363096e-06
   DEBUG:root:i=607 residual=2.414490154478699e-06
   DEBUG:root:i=608 residual=2.389912197031663e-06
   DEBUG:root:i=609 residual=2.363718067499576e-06
   DEBUG:root:i=610 residual=2.3380416678264737e-06
   DEBUG:root:i=611 residual=2.3141681140259607e-06
   DEBUG:root:i=612 residual=2.2871918190503493e-06
   DEBUG:root:i=613 residual=2.264037902932614e-06
   DEBUG:root:i=614 residual=2.2397418888431275e-06
   DEBUG:root:i=615 residual=2.215795802840148e-06
   DEBUG:root:i=616 residual=2.190646000599372e-06
   DEBUG:root:i=617 residual=2.1673620267392835e-06
   DEBUG:root:i=618 residual=2.1448095139930956e-06
   DEBUG:root:i=619 residual=2.1229423055046936e-06
   DEBUG:root:i=620 residual=2.1008504518249538e-06
   DEBUG:root:i=621 residual=2.075413021884742e-06
   DEBUG:root:i=622 residual=2.053692469417001e-06
   DEBUG:root:i=623 residual=2.035505985986674e-06
   DEBUG:root:i=624 residual=2.010661773965694e-06
   DEBUG:root:i=625 residual=1.9888475435436703e-06
   DEBUG:root:i=626 residual=1.966777972484124e-06
   DEBUG:root:i=627 residual=1.9453887034615036e-06
   DEBUG:root:i=628 residual=1.9247327145421878e-06
   DEBUG:root:i=629 residual=1.9046829038416035e-06
   DEBUG:root:i=630 residual=1.8839411950466456e-06
   DEBUG:root:i=631 residual=1.8623586583998986e-06
   DEBUG:root:i=632 residual=1.8433946706863935e-06
   DEBUG:root:i=633 residual=1.8260861907037906e-06
   DEBUG:root:i=634 residual=1.8053523263006355e-06
   DEBUG:root:i=635 residual=1.7872559965326218e-06
   DEBUG:root:i=636 residual=1.765286242516595e-06
   DEBUG:root:i=637 residual=1.7464351458329475e-06
   DEBUG:root:i=638 residual=1.7277026245210436e-06
   DEBUG:root:i=639 residual=1.709191337795346e-06
   DEBUG:root:i=640 residual=1.690419708211266e-06
   DEBUG:root:i=641 residual=1.6733289385229e-06
   DEBUG:root:i=642 residual=1.6543891661058296e-06
   DEBUG:root:i=643 residual=1.6368435353797395e-06
   DEBUG:root:i=644 residual=1.621759793124511e-06
   DEBUG:root:i=645 residual=1.6016599602153292e-06
   DEBUG:root:i=646 residual=1.5850512227189029e-06
   DEBUG:root:i=647 residual=1.5680071783208405e-06
   DEBUG:root:i=648 residual=1.551893888063205e-06
   DEBUG:root:i=649 residual=1.5353688240793417e-06
   DEBUG:root:i=650 residual=1.5234057855195715e-06
   DEBUG:root:i=651 residual=1.5039084928503144e-06
   DEBUG:root:i=652 residual=1.4903714600222884e-06
   DEBUG:root:i=653 residual=1.472985559303197e-06
   DEBUG:root:i=654 residual=1.4553172604792053e-06
   DEBUG:root:i=655 residual=1.438288677491073e-06
   DEBUG:root:i=656 residual=1.423961407454044e-06
   DEBUG:root:i=657 residual=1.4083396990827168e-06
   DEBUG:root:i=658 residual=1.3921440995545709e-06
   DEBUG:root:i=659 residual=1.377628564114275e-06
   DEBUG:root:i=660 residual=1.3622061487694737e-06
   DEBUG:root:i=661 residual=1.3502344700100366e-06
   DEBUG:root:i=662 residual=1.3351931329452782e-06
   DEBUG:root:i=663 residual=1.3175582580515766e-06
   DEBUG:root:i=664 residual=1.3037951021033223e-06
   DEBUG:root:i=665 residual=1.2896819043817231e-06
   DEBUG:root:i=666 residual=1.2781011946572107e-06
   DEBUG:root:i=667 residual=1.2664685300478595e-06
   DEBUG:root:i=668 residual=1.250762807103456e-06
   DEBUG:root:i=669 residual=1.239508264916367e-06
   DEBUG:root:i=670 residual=1.2247310223756358e-06
   DEBUG:root:i=671 residual=1.209777224175923e-06
   DEBUG:root:i=672 residual=1.1968206763413036e-06
   DEBUG:root:i=673 residual=1.183548533845169e-06
   DEBUG:root:i=674 residual=1.1708087868100847e-06
   DEBUG:root:i=675 residual=1.1576813676583697e-06
   DEBUG:root:i=676 residual=1.1483195976325078e-06
   DEBUG:root:i=677 residual=1.136680225499731e-06
   DEBUG:root:i=678 residual=1.124384652939625e-06
   DEBUG:root:i=679 residual=1.1101428754045628e-06
   DEBUG:root:i=680 residual=1.097537733585341e-06
   DEBUG:root:i=681 residual=1.0859855592570966e-06
   DEBUG:root:i=682 residual=1.0772004088721587e-06
   DEBUG:root:i=683 residual=1.067445737135131e-06
   DEBUG:root:i=684 residual=1.0557587302173488e-06
   DEBUG:root:i=685 residual=1.0439051720823045e-06
   DEBUG:root:i=686 residual=1.0295717629560386e-06
   DEBUG:root:i=687 residual=1.0178688398809754e-06
   DEBUG:root:i=688 residual=1.0062733508675592e-06
   DEBUG:root:i=689 residual=9.967058076654212e-07
   INFO:root:rank=0 pagerank=7.0150e-01 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
   INFO:root:rank=1 pagerank=7.0149e-01 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
   INFO:root:rank=2 pagerank=1.0558e-01 url=www.lawfareblog.com/cost-using-zero-days
   INFO:root:rank=3 pagerank=3.1754e-02 url=www.lawfareblog.com/lawfare-podcast-former-congressman-brian-baird-and-daniel-schuman-how-congress-can-continue-function
   INFO:root:rank=4 pagerank=2.1940e-02 url=www.lawfareblog.com/events
   INFO:root:rank=5 pagerank=1.6014e-02 url=www.lawfareblog.com/water-wars-increased-us-focus-indo-pacific
   INFO:root:rank=6 pagerank=1.6013e-02 url=www.lawfareblog.com/water-wars-drill-maybe-drill
   INFO:root:rank=7 pagerank=1.6010e-02 url=www.lawfareblog.com/water-wars-disjointed-operations-south-china-sea
   INFO:root:rank=8 pagerank=1.6008e-02 url=www.lawfareblog.com/water-wars-song-oil-and-fire
   INFO:root:rank=9 pagerank=1.6008e-02 url=www.lawfareblog.com/water-wars-sinking-feeling-philippine-china-relations
   ```

   Task 2, part 1:
   ```
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2 --personalization_vector_query='corona'
   INFO:root:rank=0 pagerank=6.3127e-01 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
   INFO:root:rank=1 pagerank=6.3124e-01 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
   INFO:root:rank=2 pagerank=1.5947e-01 url=www.lawfareblog.com/chinatalk-how-party-takes-its-propaganda-global
   INFO:root:rank=3 pagerank=1.2209e-01 url=www.lawfareblog.com/rational-security-my-corona-edition
   INFO:root:rank=4 pagerank=1.2209e-01 url=www.lawfareblog.com/brexit-not-immune-coronavirus
   INFO:root:rank=5 pagerank=9.3360e-02 url=www.lawfareblog.com/trump-cant-reopen-country-over-state-objections
   INFO:root:rank=6 pagerank=9.1920e-02 url=www.lawfareblog.com/britains-coronavirus-response
   INFO:root:rank=7 pagerank=9.1920e-02 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
   INFO:root:rank=8 pagerank=7.7770e-02 url=www.lawfareblog.com/lawfare-podcast-united-nations-and-coronavirus-crisis
   INFO:root:rank=9 pagerank=7.2888e-02 url=www.lawfareblog.com/house-oversight-committee-holds-day-two-hearing-government-coronavirus-response
   ```

   Task 2, part 2:
   ```
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2 --personalization_vector_query='corona' --search_query='-corona'
   INFO:root:rank=0 pagerank=6.3127e-01 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
   INFO:root:rank=1 pagerank=6.3124e-01 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
   INFO:root:rank=2 pagerank=1.5947e-01 url=www.lawfareblog.com/chinatalk-how-party-takes-its-propaganda-global
   INFO:root:rank=3 pagerank=9.3360e-02 url=www.lawfareblog.com/trump-cant-reopen-country-over-state-objections
   INFO:root:rank=4 pagerank=7.0277e-02 url=www.lawfareblog.com/fault-lines-foreign-policy-quarantined
   INFO:root:rank=5 pagerank=6.9713e-02 url=www.lawfareblog.com/lawfare-podcast-mom-and-dad-talk-clinical-trials-pandemic
   INFO:root:rank=6 pagerank=6.4944e-02 url=www.lawfareblog.com/limits-world-health-organization
   INFO:root:rank=7 pagerank=5.9492e-02 url=www.lawfareblog.com/chinatalk-dispatches-shanghai-beijing-and-hong-kong
   INFO:root:rank=8 pagerank=5.1245e-02 url=www.lawfareblog.com/us-moves-dismiss-case-against-company-linked-ira-troll-farm
   INFO:root:rank=9 pagerank=5.1245e-02 url=www.lawfareblog.com/livestream-house-foreign-affairs-committee-holds-hearing-crisis-idlib
   ```

# Intro PageRank-Project

In this project, you will create a simple search engine for the website <https://www.lawfareblog.com>.
This website provides legal analysis on US national security issues.
You will use pagerank to return only the most important results from this website in your search engine.

**Due date:** Sunday, 29 September at midnight

**Late Policy:** You lose $2^{(i-1)}$ points, where i is the number of days late.

<!--
**Computation:**
This project has low computational requirements.
You should be able to complete it on your own laptops.
-->

**Collaboration Policy:**
Do whatever will help you learn,
but be an adult.
You may talk to other students and use Google/ChatGPT.
Recall that you will have an in-person oral exam on this material and the exam is worth many more points.
The main purpose of this project is to help prepare you for the exam.


## Background

**Data:**

The `data` folder contains two files that store example "web graphs".
The file `small.csv.gz` contains the example graph from the *Deeper Inside Pagerank* paper.
This is a small graph, so we can manually inspect the contents of this file with the following command:
```
$ zcat data/small.csv.gz
source,target
1,2
1,3
3,1
3,2
3,5
4,5
4,6
5,6
5,4
6,4
```

> **Recall:**
> The `cat` terminal command outputs the contents of a file to stdout, and the `zcat` command first decompressed a gzipped file and then outputs the decompressed contents.
>
> In python, we can use the built-in `gzip` module to access gzipped files.
> The following python code is equivalent to the bash code above:
>
> ```
> >>> import gzip
> >>> fin = gzip.open('data/small.csv.gz', mode='rt')
> >>> print(fin.read())
> source,target
> 1,2
> 1,3
> 3,1
> 3,2
> 3,5
> 4,5
> 4,6
> 5,6
> 5,4
> 6,4
> ```
>
> There are many terminal commands throughout these instructions.
> If you haven't used the terminal before, and so these commands are unfamiliar, that's okay.
> I'd be happy to explain them in office hours,
> or there are many tutors in the QCL available who can help.
> (There are no tutors for this class specifically, but anyone who has taken CSCI046 or CSCI133 with me will be able to help with the terminal.)
>
> Furthermore, you don't "need" to understand the terminal commands in detail,
> since you are not required to run these commands or to create your own.
> The important part is to understand the English language description of what the commands are doing,
> and to understand that this is just how I computed what the English language text is describing.

As you can see, the graph is stored as a CSV file.
The first line is a header,
and each subsequent line stores a single edge in the graph.
The first column contains the source node of the edge and the second column the target node.
The file is assumed to be sorted alphabetically.

The second data file `lawfareblog.csv.gz` contains the link structure for the lawfare blog.
Let's take a look at the first 10 of these lines:
```
$ zcat data/lawfareblog.csv.gz | head
source,target
www.lawfareblog.com/,www.lawfareblog.com/topic/interrogation
www.lawfareblog.com/,www.lawfareblog.com/upcoming-events
www.lawfareblog.com/,www.lawfareblog.com/
www.lawfareblog.com/,www.lawfareblog.com/our-comments-policy
www.lawfareblog.com/,www.lawfareblog.com/litigation-documents-related-appointment-matthew-whitaker-acting-attorney-general
www.lawfareblog.com/,www.lawfareblog.com/topic/lawfare-research-paper-series
www.lawfareblog.com/,www.lawfareblog.com/topic/book-reviews
www.lawfareblog.com/,www.lawfareblog.com/documents-related-mueller-investigation
www.lawfareblog.com/,www.lawfareblog.com/topic/international-law-loac
```
You can see that in this file, the node names are URLs.
Semantically, each line corresponds to an HTML `<a>` tag that is contained in the source webpage and links to the target webpage.

We can use the following command to count the total number of links in the file:
```
$ zcat data/lawfareblog.csv.gz | wc -l
1610789
```
Since every link corresponds to a non-zero entry in the $P$ matrix,
this is also the value of $\text{nnz}(P)$.
(Technically, we should subtract 1 from this value since the `wc -l` command also counts the header line, not just the data lines.)

To get the dimensions of $P$, we need to count the total number of nodes in the graph.
The following command achieves this by: decompressing the file, extracting the first column, removing all duplicate lines, then counting the results.
```
$ zcat data/lawfareblog.csv.gz | cut -f1 -d, | uniq | wc -l
25761
```
This matrix is large enough that computing matrix products for dense matrices takes several minutes on a single CPU.
Fortunately, however, the matrix is very sparse.
The following python code computes the fraction of entries in the matrix with non-zero values:
```
>>> 1610788 / (25760**2)
0.0024274297384360172
```
Thus, by using sparse matrix operations, we will be able to speed up the code significantly.

**Code:**

The `pagerank.py` file contains code for loading the graph CSV files and searching through their nodes for key phrases.
For example, you can perform a search for all nodes (i.e. urls) that mention the string `corona` with the following command:
```
$ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --search_query=corona
```

> **NOTE:**
> It will take about 10 seconds to load and parse the data files.
> All the other computation happens essentially instantly.

Currently, the pagerank of the nodes is not currently being calculated correctly, and so the webpages are returned in an arbitrary order.
Your task in this assignment will be to fix these calculations in order to have the most important results (i.e. highest pagerank results) returned first.

## Task 1: the power method

Implement the `WebGraph.power_method` function in `pagerank.py` for computing the pagerank vector by fixing the [`FIXME: Task 1` annotation](https://github.com/mikeizbicki/cmc-csci145-math166/blob/81ed5d2b75f5bc23b8de93805c29321ab431ed9b/topic01_computation_pagerank/project/pagerank.py#L144).

> **NOTE:**
> The power method is the only data mining algorithm you will implement in class.
> You are implementing it because there are no standard library implementations available.
> Why?
> 1. The runtime is heavily dependent on the data structures used to store the graph data.
>    Different applications will need to use different data structures.
> 1. It is "trivial" to implement.
>    My solution to this homework is <10 lines of code.

**Part 1:**

To check that your implementation is working,
you should run the program on the `data/small.csv.gz` graph.
For my implementation, I get the following output.
```
$ python3 pagerank.py --data=data/small.csv.gz --verbose
DEBUG:root:computing indices
DEBUG:root:computing values
DEBUG:root:i=0 residual=2.5629e-01
DEBUG:root:i=1 residual=1.1841e-01
DEBUG:root:i=2 residual=7.0701e-02
DEBUG:root:i=3 residual=3.1815e-02
DEBUG:root:i=4 residual=2.0497e-02
DEBUG:root:i=5 residual=1.0108e-02
DEBUG:root:i=6 residual=6.3716e-03
DEBUG:root:i=7 residual=3.4228e-03
DEBUG:root:i=8 residual=2.0879e-03
DEBUG:root:i=9 residual=1.1750e-03
DEBUG:root:i=10 residual=7.0131e-04
DEBUG:root:i=11 residual=4.0321e-04
DEBUG:root:i=12 residual=2.3800e-04
DEBUG:root:i=13 residual=1.3812e-04
DEBUG:root:i=14 residual=8.1083e-05
DEBUG:root:i=15 residual=4.7251e-05
DEBUG:root:i=16 residual=2.7704e-05
DEBUG:root:i=17 residual=1.6164e-05
DEBUG:root:i=18 residual=9.4778e-06
DEBUG:root:i=19 residual=5.5066e-06
DEBUG:root:i=20 residual=3.2042e-06
DEBUG:root:i=21 residual=1.8612e-06
DEBUG:root:i=22 residual=1.1283e-06
DEBUG:root:i=23 residual=6.1907e-07
INFO:root:rank=0 pagerank=6.6270e-01 url=4
INFO:root:rank=1 pagerank=5.2179e-01 url=6
INFO:root:rank=2 pagerank=4.1434e-01 url=5
INFO:root:rank=3 pagerank=2.3175e-01 url=2
INFO:root:rank=4 pagerank=1.8590e-01 url=3
INFO:root:rank=5 pagerank=1.6917e-01 url=1
```
Yours likely won't be identical (due to minor implementation details and weird floating point issues), but it should be similar.
In particular, the ranking of the nodes/urls should be the same order.

> **NOTE:**
> The `--verbose` flag causes all of the lines beginning with `DEBUG` to be printed.
> By default, only lines beginning with `INFO` are printed.

> **NOTE:**
> There are no automated test cases to pass for this assignment.
> Test cases for algorithms involving floating point computations are hard to write and understand.
> Minor-seeming implementations details can have large impacts on the final result.
> These software engineering issues are beyond the scope of this class.
>
> Instructions for how I will grade your homework are contained in the [submission section](#submission) at the end of this document.

**Part 2:**

The `pagerank.py` file has an option `--search_query`, which takes a string as a parameter.
If this argument is used, then the program returns all nodes that match the query string sorted according to their pagerank.
Essentially, this gives us the most important pages related to our query.

Again, you may not get the exact same results as me,
but you should get similar results to the examples I've shown below.
Verify that you do in fact get similar results.

```
$ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='corona'
INFO:root:rank=0 pagerank=1.0038e-03 url=www.lawfareblog.com/lawfare-podcast-united-nations-and-coronavirus-crisis
INFO:root:rank=1 pagerank=8.9224e-04 url=www.lawfareblog.com/house-oversight-committee-holds-day-two-hearing-government-coronavirus-response
INFO:root:rank=2 pagerank=7.0390e-04 url=www.lawfareblog.com/britains-coronavirus-response
INFO:root:rank=3 pagerank=6.9153e-04 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
INFO:root:rank=4 pagerank=6.7041e-04 url=www.lawfareblog.com/israeli-emergency-regulations-location-tracking-coronavirus-carriers
INFO:root:rank=5 pagerank=6.6256e-04 url=www.lawfareblog.com/why-congress-conducting-business-usual-face-coronavirus
INFO:root:rank=6 pagerank=6.5046e-04 url=www.lawfareblog.com/congressional-homeland-security-committees-seek-ways-support-state-federal-responses-coronavirus
INFO:root:rank=7 pagerank=6.3620e-04 url=www.lawfareblog.com/paper-hearing-experts-debate-digital-contact-tracing-and-coronavirus-privacy-concerns
INFO:root:rank=8 pagerank=6.1248e-04 url=www.lawfareblog.com/house-subcommittee-voices-concerns-over-us-management-coronavirus
INFO:root:rank=9 pagerank=6.0187e-04 url=www.lawfareblog.com/livestream-house-oversight-committee-holds-hearing-government-coronavirus-response

$ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='trump'
INFO:root:rank=0 pagerank=5.7826e-03 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
INFO:root:rank=1 pagerank=5.2338e-03 url=www.lawfareblog.com/document-trump-revokes-obama-executive-order-counterterrorism-strike-casualty-reporting
INFO:root:rank=2 pagerank=5.1297e-03 url=www.lawfareblog.com/trump-administrations-worrying-new-policy-israeli-settlements
INFO:root:rank=3 pagerank=4.6599e-03 url=www.lawfareblog.com/dc-circuit-overrules-district-courts-due-process-ruling-qasim-v-trump
INFO:root:rank=4 pagerank=4.5934e-03 url=www.lawfareblog.com/donald-trump-and-politically-weaponized-executive-branch
INFO:root:rank=5 pagerank=4.3071e-03 url=www.lawfareblog.com/how-trumps-approach-middle-east-ignores-past-future-and-human-condition
INFO:root:rank=6 pagerank=4.0935e-03 url=www.lawfareblog.com/why-trump-cant-buy-greenland
INFO:root:rank=7 pagerank=3.7591e-03 url=www.lawfareblog.com/oral-argument-summary-qassim-v-trump
INFO:root:rank=8 pagerank=3.4509e-03 url=www.lawfareblog.com/dc-circuit-court-denies-trump-rehearing-mazars-case
INFO:root:rank=9 pagerank=3.4484e-03 url=www.lawfareblog.com/second-circuit-rules-mazars-must-hand-over-trump-tax-returns-new-york-prosecutors

$ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='iran'
INFO:root:rank=0 pagerank=4.5746e-03 url=www.lawfareblog.com/praise-presidents-iran-tweets
INFO:root:rank=1 pagerank=4.4174e-03 url=www.lawfareblog.com/how-us-iran-tensions-could-disrupt-iraqs-fragile-peace
INFO:root:rank=2 pagerank=2.6928e-03 url=www.lawfareblog.com/cyber-command-operational-update-clarifying-june-2019-iran-operation
INFO:root:rank=3 pagerank=1.9391e-03 url=www.lawfareblog.com/aborted-iran-strike-fine-line-between-necessity-and-revenge
INFO:root:rank=4 pagerank=1.5452e-03 url=www.lawfareblog.com/parsing-state-departments-letter-use-force-against-iran
INFO:root:rank=5 pagerank=1.5357e-03 url=www.lawfareblog.com/iranian-hostage-crisis-and-its-effect-american-politics
INFO:root:rank=6 pagerank=1.5258e-03 url=www.lawfareblog.com/announcing-united-states-and-use-force-against-iran-new-lawfare-e-book
INFO:root:rank=7 pagerank=1.4221e-03 url=www.lawfareblog.com/us-names-iranian-revolutionary-guard-terrorist-organization-and-sanctions-international-criminal
INFO:root:rank=8 pagerank=1.1788e-03 url=www.lawfareblog.com/iran-shoots-down-us-drone-domestic-and-international-legal-implications
INFO:root:rank=9 pagerank=1.1463e-03 url=www.lawfareblog.com/israel-iran-syria-clash-and-law-use-force
```

**Part 3:**

The webgraph of lawfareblog.com (i.e. the $P$ matrix) naturally contains a lot of structure.
For example, essentially all pages on the domain have links to the root page <https://lawfareblog.com/> and other "non-article" pages like <https://www.lawfareblog.com/topics> and <https://www.lawfareblog.com/subscribe-lawfare>.
These pages therefore have a large pagerank.
We can get a list of the pages with the largest pagerank by running

```
$ python3 pagerank.py --data=data/lawfareblog.csv.gz
INFO:root:rank=0 pagerank=2.8741e-01 url=www.lawfareblog.com/lawfare-job-board
INFO:root:rank=1 pagerank=2.8741e-01 url=www.lawfareblog.com/masthead
INFO:root:rank=2 pagerank=2.8741e-01 url=www.lawfareblog.com/litigation-documents-related-appointment-matthew-whitaker-acting-attorney-general
INFO:root:rank=3 pagerank=2.8741e-01 url=www.lawfareblog.com/documents-related-mueller-investigation
INFO:root:rank=4 pagerank=2.8741e-01 url=www.lawfareblog.com/topics
INFO:root:rank=5 pagerank=2.8741e-01 url=www.lawfareblog.com/about-lawfare-brief-history-term-and-site
INFO:root:rank=6 pagerank=2.8741e-01 url=www.lawfareblog.com/snowden-revelations
INFO:root:rank=7 pagerank=2.8741e-01 url=www.lawfareblog.com/support-lawfare
INFO:root:rank=8 pagerank=2.8741e-01 url=www.lawfareblog.com/upcoming-events
INFO:root:rank=9 pagerank=2.8741e-01 url=www.lawfareblog.com/our-comments-policy
```

Most of these pages are not very interesting, however, because they are not articles,
and usually when we are performing a web search, we only want articles.

This raises the question: How can we find the most important articles filtering out the non-article pages?
The answer is to modify the $P$ matrix by removing all links to non-article pages.

This raises another question: How do we know if a link is a non-article page?
Unfortunately, this is a hard question to answer with 100% accuracy,
but there are many methods that get us most of the way there.
One easy to implement method is to compute what's called the "in-link ratio" of each node (i.e. the total number of edges with the node as a target divided by the total number of nodes),
and then remove nodes from the search results with too-high of a ratio.
The intuition is that non-article pages often appear in the menu of a webpage, and so have links from almost all of the other webpages;
but article-webpages are unlikely to appear on a menu and so will only have a small number of links from other webpages.
The `--filter_ratio` parameter causes the code to remove all pages that have an in-link ratio larger than the provided value.

Using this option, we can estimate the most important articles on the domain with the following command:
```
$ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2
INFO:root:rank=0 pagerank=3.4696e-01 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
INFO:root:rank=1 pagerank=2.9521e-01 url=www.lawfareblog.com/livestream-nov-21-impeachment-hearings-0
INFO:root:rank=2 pagerank=2.9040e-01 url=www.lawfareblog.com/opening-statement-david-holmes
INFO:root:rank=3 pagerank=1.5179e-01 url=www.lawfareblog.com/lawfare-podcast-ben-nimmo-whack-mole-game-disinformation
INFO:root:rank=4 pagerank=1.5099e-01 url=www.lawfareblog.com/todays-headlines-and-commentary-1963
INFO:root:rank=5 pagerank=1.5099e-01 url=www.lawfareblog.com/todays-headlines-and-commentary-1964
INFO:root:rank=6 pagerank=1.5071e-01 url=www.lawfareblog.com/lawfare-podcast-week-was-impeachment
INFO:root:rank=7 pagerank=1.4957e-01 url=www.lawfareblog.com/todays-headlines-and-commentary-1962
INFO:root:rank=8 pagerank=1.4367e-01 url=www.lawfareblog.com/cyberlaw-podcast-mistrusting-google
INFO:root:rank=9 pagerank=1.4240e-01 url=www.lawfareblog.com/lawfare-podcast-bonus-edition-gordon-sondland-vs-committee-no-bull
```
Notice that the urls in this list look much more like articles than the urls in the previous list.

When Google calculates their $P$ matrix for the web,
they use a similar (but much more complicated) process to modify the $P$ matrix in order to reduce spam results.
The exact formula they use is a jealously guarded secret that they update continuously.

In the case above, notice that we have accidentally removed the blog's most popular article (<https://www.lawfareblog.com/snowden-revelations>).
The blog editors believed that Snowden's revelations about NSA spying are so important that they directly put a link to the article on the menu.
So every single webpage in the domain links to the Snowden article,
and our "anti-spam" `--filter-ratio` argument removed this article from the list.
In general, it is a challenging open problem to remove spam from pagerank results,
and all current solutions rely on careful human tuning and still have lots of false positives and false negatives.

**Part 4:**

Recall from the reading that the runtime of pagerank depends heavily on the eigengap of the $\bar{\bar P}$ matrix,
and that this eigengap is bounded by the alpha parameter.

Run the following four commands:
```
$ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose 
$ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --alpha=0.99999
$ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --filter_ratio=0.2
$ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --filter_ratio=0.2 --alpha=0.99999
```
You should notice that the last command takes considerably more iterations to compute the pagerank vector.
(My code takes 685 iterations for this call, and about 10 iterations for all the others.)

This raises the question: Why does the second command (with the `--alpha` option but without the `--filter_ratio`) option not take a long time to run?
The answer is that the $P$ graph for <https://www.lawfareblog.com> naturally has a large eigengap and so is fast to compute for all alpha values,
but the modified graph does not have a large eigengap and so requires a small alpha for fast convergence.

Changing the value of alpha also gives us very different pagerank rankings.
For example, 
```
$ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2
INFO:root:rank=0 pagerank=3.4696e-01 url=www.lawfareblog.com/trump-asks-supreme-court-stay-congressional-subpeona-tax-returns
INFO:root:rank=1 pagerank=2.9521e-01 url=www.lawfareblog.com/livestream-nov-21-impeachment-hearings-0
INFO:root:rank=2 pagerank=2.9040e-01 url=www.lawfareblog.com/opening-statement-david-holmes
INFO:root:rank=3 pagerank=1.5179e-01 url=www.lawfareblog.com/lawfare-podcast-ben-nimmo-whack-mole-game-disinformation
INFO:root:rank=4 pagerank=1.5099e-01 url=www.lawfareblog.com/todays-headlines-and-commentary-1963
INFO:root:rank=5 pagerank=1.5099e-01 url=www.lawfareblog.com/todays-headlines-and-commentary-1964
INFO:root:rank=6 pagerank=1.5071e-01 url=www.lawfareblog.com/lawfare-podcast-week-was-impeachment
INFO:root:rank=7 pagerank=1.4957e-01 url=www.lawfareblog.com/todays-headlines-and-commentary-1962
INFO:root:rank=8 pagerank=1.4367e-01 url=www.lawfareblog.com/cyberlaw-podcast-mistrusting-google
INFO:root:rank=9 pagerank=1.4240e-01 url=www.lawfareblog.com/lawfare-podcast-bonus-edition-gordon-sondland-vs-committee-no-bull

$ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2 --alpha=0.99999
INFO:root:rank=0 pagerank=7.0149e-01 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
INFO:root:rank=1 pagerank=7.0149e-01 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
INFO:root:rank=2 pagerank=1.0552e-01 url=www.lawfareblog.com/cost-using-zero-days
INFO:root:rank=3 pagerank=3.1755e-02 url=www.lawfareblog.com/lawfare-podcast-former-congressman-brian-baird-and-daniel-schuman-how-congress-can-continue-function
INFO:root:rank=4 pagerank=2.2040e-02 url=www.lawfareblog.com/events
INFO:root:rank=5 pagerank=1.6027e-02 url=www.lawfareblog.com/water-wars-increased-us-focus-indo-pacific
INFO:root:rank=6 pagerank=1.6026e-02 url=www.lawfareblog.com/water-wars-drill-maybe-drill
INFO:root:rank=7 pagerank=1.6023e-02 url=www.lawfareblog.com/water-wars-disjointed-operations-south-china-sea
INFO:root:rank=8 pagerank=1.6020e-02 url=www.lawfareblog.com/water-wars-song-oil-and-fire
INFO:root:rank=9 pagerank=1.6020e-02 url=www.lawfareblog.com/water-wars-sinking-feeling-philippine-china-relations
```

Which of these rankings is better is entirely subjective,
and the only way to know if you have the "best" alpha for your application is to try several variations and see what is best.

> **NOTE:**
> It should be "obvious" to you that large alpha values imply that the structure of the webgraph has more influence on the final result,
> and small alpha values ignore the structure of the webgraph.
> Recall that the word "obvious" means that it follows directly from the definition,
> but you may still need to sit and meditate on the definition for a long period of time.

If large alphas are good for your application, you can see that there is a trade-off between quality answers and algorithmic runtime.
We'll be exploring this trade-off more formally in class over the rest of the semester.

## Task 2: the personalization vector

The most interesting applications of pagerank involve the personalization vector.
Implement the `WebGraph.make_personalization_vector` function so that it outputs a personalization vector tuned for the input query.
The pseudocode for the function is:
```
for each index in the personalization vector:
    get the url for the index (see the _index_to_url function)
    check if the url satisfies the input query (see the url_satisfies_query function)
    if so, set the corresponding index to one
normalize the vector
```

**Part 1:**

The command line argument `--personalization_vector_query` will use the function you created above to augment your search with a custom personalization vector.
If you've implemented the function correctly,
you should get results similar to:
```
$ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2 --personalization_vector_query='corona'
INFO:root:rank=0 pagerank=6.3127e-01 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
INFO:root:rank=1 pagerank=6.3124e-01 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
INFO:root:rank=2 pagerank=1.5947e-01 url=www.lawfareblog.com/chinatalk-how-party-takes-its-propaganda-global
INFO:root:rank=3 pagerank=1.2209e-01 url=www.lawfareblog.com/brexit-not-immune-coronavirus
INFO:root:rank=4 pagerank=1.2209e-01 url=www.lawfareblog.com/rational-security-my-corona-edition
INFO:root:rank=5 pagerank=9.3360e-02 url=www.lawfareblog.com/trump-cant-reopen-country-over-state-objections
INFO:root:rank=6 pagerank=9.1920e-02 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
INFO:root:rank=7 pagerank=9.1920e-02 url=www.lawfareblog.com/britains-coronavirus-response
INFO:root:rank=8 pagerank=7.7770e-02 url=www.lawfareblog.com/lawfare-podcast-united-nations-and-coronavirus-crisis
INFO:root:rank=9 pagerank=7.2888e-02 url=www.lawfareblog.com/house-oversight-committee-holds-day-two-hearing-government-coronavirus-response
```

Notice that these results are significantly different than when using the `--search_query` option:
```
$ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2 --search_query='corona'
INFO:root:rank=0 pagerank=8.1320e-03 url=www.lawfareblog.com/house-oversight-committee-holds-day-two-hearing-government-coronavirus-response
INFO:root:rank=1 pagerank=7.7908e-03 url=www.lawfareblog.com/lawfare-podcast-united-nations-and-coronavirus-crisis
INFO:root:rank=2 pagerank=5.2262e-03 url=www.lawfareblog.com/livestream-house-oversight-committee-holds-hearing-government-coronavirus-response
INFO:root:rank=3 pagerank=3.9584e-03 url=www.lawfareblog.com/britains-coronavirus-response
INFO:root:rank=4 pagerank=3.8114e-03 url=www.lawfareblog.com/prosecuting-purposeful-coronavirus-exposure-terrorism
INFO:root:rank=5 pagerank=3.3973e-03 url=www.lawfareblog.com/paper-hearing-experts-debate-digital-contact-tracing-and-coronavirus-privacy-concerns
INFO:root:rank=6 pagerank=3.3633e-03 url=www.lawfareblog.com/cyberlaw-podcast-how-israel-fighting-coronavirus
INFO:root:rank=7 pagerank=3.3557e-03 url=www.lawfareblog.com/israeli-emergency-regulations-location-tracking-coronavirus-carriers
INFO:root:rank=8 pagerank=3.2160e-03 url=www.lawfareblog.com/congress-needs-coronavirus-failsafe-its-too-late
INFO:root:rank=9 pagerank=3.1036e-03 url=www.lawfareblog.com/why-congress-conducting-business-usual-face-coronavirus
```

Which results are better?
Again, that depends on what you mean by "better."
With the `--personalization_vector_query` option,
a webpage is important only if other coronavirus webpages also think it's important;
with the `--search_query` option,
a webpage is important if any other webpage thinks it's important.
You'll notice that in the later example, many of the webpages are about Congressional proceedings related to the coronavirus.
From a strictly coronavirus perspective, these are not very important webpages.
But in the broader context of national security, these are very important webpages.

Google engineers spend TONs of time fine-tuning their pagerank personalization vectors to remove spam webpages.
Exactly how they do this is another one of their secrets that they don't publicly talk about.

**Part 2:**

Another use of the `--personalization_vector_query` option is that we can find out what webpages are related to the coronavirus but don't directly mention the coronavirus.
This can be used to map out what types of topics are similar to the coronavirus.

For example, the following query ranks all webpages by their `corona` importance,
but removes webpages mentioning `corona` from the results.
```
$ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2 --personalization_vector_query='corona' --search_query='-corona'
INFO:root:rank=0 pagerank=6.3127e-01 url=www.lawfareblog.com/covid-19-speech-and-surveillance-response
INFO:root:rank=1 pagerank=6.3124e-01 url=www.lawfareblog.com/lawfare-live-covid-19-speech-and-surveillance
INFO:root:rank=2 pagerank=1.5947e-01 url=www.lawfareblog.com/chinatalk-how-party-takes-its-propaganda-global
INFO:root:rank=3 pagerank=9.3360e-02 url=www.lawfareblog.com/trump-cant-reopen-country-over-state-objections
INFO:root:rank=4 pagerank=7.0277e-02 url=www.lawfareblog.com/fault-lines-foreign-policy-quarantined
INFO:root:rank=5 pagerank=6.9713e-02 url=www.lawfareblog.com/lawfare-podcast-mom-and-dad-talk-clinical-trials-pandemic
INFO:root:rank=6 pagerank=6.4944e-02 url=www.lawfareblog.com/limits-world-health-organization
INFO:root:rank=7 pagerank=5.9492e-02 url=www.lawfareblog.com/chinatalk-dispatches-shanghai-beijing-and-hong-kong
INFO:root:rank=8 pagerank=5.1245e-02 url=www.lawfareblog.com/us-moves-dismiss-case-against-company-linked-ira-troll-farm
INFO:root:rank=9 pagerank=5.1245e-02 url=www.lawfareblog.com/livestream-house-armed-services-holds-hearing-national-security-challenges-north-and-south-america
```
You can see that there are many urls about concepts that are obviously related like "covid", "clinical trials", and "quarantine",
but this algorithm also finds articles about Chinese propaganda and Trump's policy decisions.
Both of these articles are highly relevant to coronavirus discussions,
but a simple keyword search for corona or related terms would not find these articles.
The vast majority of industry data mining work is finding clever uses of standard algorithms.

<!--
**Part 3:**

Select another topic related to national security.
You should experiment with a national security topic other than the coronavirus.
For example, find out what articles are important to the `iran` topic but do not contain the word `iran`.
Your goal should be to discover what topics that www.lawfareblog.com considers to be related to the national security topic you choose.
-->

## Submission

1. Create a new repo on github (not a fork of this repo).
    Ensure that all of the project files are copied from this folder into your new repo.

1. As you complete the tasks above:
    Run the corresponding commands below, and paste their output into the code blocks.
    Please ensure correct markdown formatting.
   
   Task 1, part 1:
   ```
   $ python3 pagerank.py --data=data/small.csv.gz --verbose
   ```

   Task 1, part 2:
   ```
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='corona'

   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='trump'

   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --search_query='iran'
   ```

   Task 1, part 3:
   ```
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz

   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2
   ```

   Task 1, part 4:
   ```
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose 
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --alpha=0.99999
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --filter_ratio=0.2
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --verbose --filter_ratio=0.2 --alpha=0.99999
   ```

   Task 2, part 1:
   ```
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2 --personalization_vector_query='corona'
   ```

   Task 2, part 2:
   ```
   $ python3 pagerank.py --data=data/lawfareblog.csv.gz --filter_ratio=0.2 --personalization_vector_query='corona' --search_query='-corona'
   ```

1. Ensure that all your changes to the `pagerank.py` and `README.md` files are committed to your repo and pushed to github.

1. Get at least 5 stars on your repo.
   (You may trade stars with other students in the class.)

   > **NOTE:**
   > 
   > Recruiters use github profiles to determine who to hire,
   > and pagerank is used to rank user profiles and projects.
   > Links in this graph correspond to who has starred/followed who's repo.
   > By getting more stars on your repo, you'll be increasing your github pagerank, which increases the likelihood that recruiters will hire you.
   > To see an example, [perform a search for `data mining`](https://github.com/search?q=data+mining).
   > Notice that the results are returned "approximately" ranked by the number of stars,
   > but because "some stars count more than others" the results are not exactly ranked by the number of stars.
   > (I asked you not to fork this repo because forks are ranked lower than non-forks.)
   >
   > In some sense, we are doing a "dual problem" to data mining by getting these stars.
   > Recruiters are using data mining to find out who the best people to recruit are,
   > and we are hacking their data mining algorithms by making those algorithms select you instead of someone else.
   >
   > If you're interested in exploring this idea further, here's a python tutorial for extracting GitHub's social graph: <https://www.oreilly.com/library/view/mining-the-social/9781449368180/ch07.html> ; if you're interested in learning more about how recruiters use github profiles, read this Hacker News post: <https://news.ycombinator.com/item?id=19413348>.

1. Submit the url of your repo to sakai.

   The assignment is worth 8 points.
   1. There are 6 parts to the output above.  (4 in Task1 and 2 in Task2.)
   1. Each part that you get incorrect will result in -2 points.  (But you cannot go negative.)
   1. Another way of phrasing this is that the first 2 parts you complete are not worth any points,
      but each part after that is worth 2 points.
