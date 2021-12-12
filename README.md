# MINA---P2P-O2C---Snapp

This is my result of the MINA-bootcamp, i was eletcted to join. The result is not a hack, solution or whatever other the like expected.

What i'm trying is to establish a new realm of use-cases, based on the MINA-promises of Snapps: boring Business-to-Business processes. 
While this will not make the world a better place (except perhaps for those already established), it is a critical demand for todays 
supply-chains and the backend-processing of their steps.

1. Todays blockchains are for 95% DeFi-oriented - their "native" realm, boiling down to just ordinary money speculation, using a rather 
   new technology.
   
2. Staying within the "business" realm, it is astonishing, that the processes "backing" this economy - money doesn't grow out of thin 
   air, although it sometimes looks like so -, are completely underrated and therefore underrepresented in the blockchain space. The amount
   of (non-chained) transactions in this area is estimated to be 2,5 - 3,5 trillion a year. Compared to this, DeFi is kind of cute and tiny.
   And all of these "trillion" instaces represent value/investment...
   (And hey: this is setting a new dimensioned benchmark perspective wrt to tps, right?). Anyway...
   
3. What i would like to implement on MINA, is the complete (automated) process steps of a Procure-to-Pay process (the buyers view), and
   the corresponding Order-to-Cash process (from a vendors view) between backend systems of enterprises, e.g. ERP-Systems. I have a prototype
   solution running on a Ethereum-based BESU-network. It's private/permissioned at the moment, but that doesn't matter for it's inner "ticking"
   in principle (and smootly abstracts for open questions like "gas"-costs, tps, L2-questions and the like...). Now heading for a public 
   chain - MINA's ZKP-design-priciples being the (only) appropriate candidate, as far as i see: businesses hate "publicity", and never will
   use a public chain, where a sophisticated "Mr. Robot" can put appropriate markers to gain insight into their competion-standings...
   
4. The prototype implements a Finit-State-Machine Smart-Contract w/ nine (or so) defined states, the processes named above are in per instance.
   It controls the allowed next steps (or their declinements) until reaching the FSM-end: from 'Order placed' over 'Order accepted', 'Delivery
   executed', 'Delivery accepted' to 'Bill issued' and 'Vendor invoice accepted'. Payment and any kind of Token/Tokenisation are out of scope.
   This is - imho - not a lack of features, but a nice attribute of the use case: except for tx-payments, one doesn't need to care about the
   crypto space speculation/ups-and-downs...
   
5. While the Snapp i think of would be the (kind of hidden although) core part of the whole scenario, it's completely embedded into ERP-System-
   orchestration of the respective Snapp-participants: Orders (from a buyer) are automatically prooved and posted at a vendor system, shipments
   are automatically posted at a carriers system and so on until billing/invoicing. The crucial part is: all steps are immutably saved and 
   committed to on MINA (dispute reduction), and as Snapps live off-chain, with ZKP's the complete privacy of (fierce) competitive information 
   is guaranteed.
   
As said, this is my "solution" of the bootcamp-attendance: all open tasks to be implemented. Best i can do as o non-dev, but an ERP-architect 
(Enterprise resource planning systems are kind of the "Finite-Field" of my technical thoughts; they always wrap around this: "modulo ERP"...).

I didn't plan to submit this, and i'm not in for any incentives/rewards or the like: just want to have established a new realm of use-cases
for MINA. In writing this, i have changed my opinion: whenever the above receives any reward, it should/would be staked. Not to the MINA-
net, but to "Medicine-sans-Frontiers". Unfortunately i can't commit to this yet: Snapps are not even on testnet afaik. But time will come...

Kind regards to the decicion commitee, or whatever you call this, Joerg.

