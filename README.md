# EcoAI
Age of empires 2 AI development
(defrule
	;(dropsite-min-distance deer-hunting > 50)
   (dropsite-min-distance deer-hunting != -1)
	(civilian-population > 10)
	(unit-type-count villager-hunter == 0)
	;(strategic-number sn-enable-boar-hunting != 2)
=>
   (build mill)
   (chat-to-all "deer-hunting")
	(set-strategic-number sn-minimum-number-hunters 6)
   )
