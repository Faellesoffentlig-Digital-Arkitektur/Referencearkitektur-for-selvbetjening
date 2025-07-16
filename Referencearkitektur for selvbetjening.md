# Referencearkitektur for selvbetjening

## Forord

Denne referencearkitektur er udarbejdet som led i realiseringen af initiativerne i de fællesoffentlige digitaliseringsstrategier.

Fællesoffentlig referencearkitektur for selvbetjening skal bidrage til at målrette indsatsen for at skabe sammenhængende, effektive, sikre og brugervenlige løsninger for borgere og virksomheder og økonomiske gevinster i de offentlige myndigheder, fx gennem færre supporthenvendelser og et bedre samspil mellem forskellige myndigheders selvbetjeningsløsninger. 

Referencearkitekturen skal fungere som basis for en fælles forståelse af forretningsarkitekturen, herunder de processer og begreber der er knyttet til ”digital selvbetjening”. De fælles begreber skal understøtte en bedre dialog mellem myndigheder og i forhold til leverandører i anskaffelsesprocesser. Derudover skal arkitekturen fungere som et teknisk pejlemærke for udvikling af digitale løsninger generelt i den offentlige sektor, herunder for udvikling af fælles standarder og løsninger. Den har en tæt relation til andre referencearkitekturer og den fællesoffentlige digitale arkitektur, også kaldet FDA. 

Denne referencearkitektur for selvbetjening er udarbejdet i et samarbejde mellem myndigheder med mange års erfaring med selvbetjeningsløsninger. Der vil være behov for løbende at udarbejde nye versioner af referencearkitekturen, i takt med at myndighederne indhenter erfaringer med at anvende referencearkitekturen - og i takt med at der udvikles fælles komponenter som et led i denne og andre referencearkitekturer.

## Resumé

Med selvbetjening menes i dette dokument digital selvbetjening med fokus på interaktiv, internetbaseret kommunikation.

Offentlig digital selvbetjening har traditionelt haft fokus på indsamling af data til den enkelte myndighed. En traditionel løsning har i stort omfang videreført de funktioner, som papirblanketteten har haft. Det offentlige Danmark har i de seneste år investeret i mere brugervenlige og effektive selvbetjeningsløsninger som led i udmøntningen af lovgivning omkring obligatorisk digital selvbetjening (bølgeplanerne) og har flyttet en stor del af de analoge henvendelser til myndighederne over på de digitale løsninger. Den videre udvikling af selvbetjeningsløsninger vil kræve fokus på at skabe bedre sammenhæng for brugeren i de situationer, hvor løsningen af brugerens livssituationer kræver flere selvbetjeningsløsninger. Ligeledes kan løsningerne udvikles til bedre at understøtte de øvrige opgaver, som borgeren eller virksomheden måtte have i forbindelse med den opgave, som selvbetjeningen indgår i. 

Denne referencearkitektur har til formål at skabe rammerne for både en større brugertilfredshed og en større effektivitet i den samlede opgaveløsning. Her tænkes på forhold, som i højere grad understøtter borgerens eller virksomhedens samlede opgaver og behov, en højere grad af genbrug og en bedre integration til fagsystemer m.m. Det er forhold, som kan befordre bedre sammenhæng mellem flere selvbetjeningsløsninger, når brugeren står i en livssituation, hvor en række forskellige selvbetjeningsløsninger skal anvendes, for at brugerens samlede behov kan opfyldes gennem selvbetjening. Dette kan blandt andet ske ved at øge automatiseringsgraden, så en større del af processen – og på nogle få områder hele processen – kan gennemføres uden at involvere en sagsbehandler og derved eventuelt  resultere i straksafgørelser.

Endelig giver udviklingen i og udbredelsen af mobile enheder (devices, apparater) mulighed for nye former for interaktivitet.

Denne referencearkitektur gør brugerrejsen til en ramme for tilrettelæggelse af selvbetjeningsforløbet, hvor perspektivet er at indføre brugeren i den opgave, der skal løses med selvbetjening, understøtte smidig og brugervenlig løsning af opgaven og med klar besked om, hvad der derefter skal ske. I denne referencearkitektur forstås brugerrejse som en brugers oplevelse af et selvbetjeningsforløb eller en selvbetjeningskæde, en kæde af forskellige, dog sammenhængende selvbetjeningsforløb. Der er tale om en mere snæver forståelse af begrebet brugerrejse, end der normalt gælder inden for servicedesign.

Med myndighedens og arkitektens perspektiv beskrives det som et selvbetjeningsforløb med forberedelse af brugeren, gennemførelse af kernen i selvbetjeningsforløbet og afrunding af selvbetjeningsforløbet. Forberedelse skal afklare og styrke brugerens forståelse af den opgave, der skal løses. Kernen er der, hvor opgaven løses, såsom at læse og godkende, ansøge, indberette og lign. Afrunding skal sikre, at brugeren er klar over, hvad gennemførelsen af kernen har bibragt brugeren, og hvilke muligheder denne nye kontekst har for brugeren. 

Referencearkitekturen beskriver desuden rammerne for, at brugerrejser, der omfatter flere selvbetjeningsforløb, kan kædes sammen i selvbetjeningskæder med efterfølgende større brugertilfredshed. Selvbetjeningsforløb kædes sammen gennem overdragelse, og referencearkitekturen tager højde for, at overdragelse kan ske mellem forskellige ressortområder.

En selvbetjeningsløsning er den eller de tekniske løsninger, der implementerer et selvbetjeningsforløb.

Referencearkitekturen for selvbetjening fastlægger en række principper for at styre frem mod en fælles forretnings- og it-arkitektur for det offentliges selvbetjeningsløsninger, men tager udgangspunkt i de fællesoffentlige princippper, her arkitekturregel 2.4 "Byg forandringsparat med udgangspunkt i brugeren" og 5.1 "Design sammenhængende brugerrejser" :

Principper for selvbetjening

1. Brugerne møder i det enkelte selvbetjeningsforløb både forberedelse, kernen og afrunding, understøttet af digitale løsninger, der imødekommer brugernes behov.
2. Selvbetjeningsløsninger er forståelige, nemme og intuitive at anvende for brugerne
3. Brugerne leverer kun information, som det offentlige ikke allerede har.
4. Brugerne oplever en sammenhængende service, også på tværs af myndigheder.
5. Brugerne skal altid kunne se, hvilken myndighed der er ansvarlig for at levere en tjeneste.
6. Myndigheder, der samarbejder om at kæde selvbetjeningsforløb sammen, aftaler opgave- og ansvarsfordeling inden for gældende regler.

De centrale tjenester realiserer følgende kapabiliteter i referencearkitekturen:

* Forberedelse
* Kernen
* Afrunding
* Overdragelse (som håndterer overdragelsen fra et selvbetjeningsforløb til det næste).

Kapabiliteterne realiserer tilsammen et selvbetjeningsforløb og anvendes af borgere eller af medarbejdere i virksomheder og kan også igangsættes af en hændelse, fx i et fagsystem. Kapabiliteter trækker på en række beskrevne funktionaliteter og vedligeholder en selvbetjeningskontekst, så et selvbetjeningsforløb kan pauses og genoptages. Skal der ske en overdragelse, beskrives, hvilke aftaler, der skal etableres, for at dette kan ske. Kapabiliteterne kan trække på informationer fra fagsystemer, brugerprofiler og fra fællesoffentlig infrastruktur som grunddata, brugerstyring (identitet og login) og andet. Se Figur 5. Kapabiliteter og aktører i selvbetjeningsforløb og selvbetjeningskæder

Referencearkitekturen anviser, hvilke softwarekomponenter der medgår i konstruktionen af selvbetjeningsløsninger, og hvilke fællesoffentlige infrastrukturkomponenter som selvbetjeningsløsningen vil trække på. Se Figur 16. Mulige komponenter i selvbetjeningsforløb. Referencearkitekturen lister de softwareteknologier, der findes på markedet til opbygning og realisering af selvbetjeningsløsninger. 

Referencearkitekturen stiller krav til de fællesoffentlige infrastrukturkomponenter og foreslår også nye. Referencearkitekturen udpeger, hvilke eksisterende standarder som skal anvendes, og hvilke nye standarder der skal udarbejdes. Referencearkitekturen gennemgår de sikkerhedsproblemstillinger, der er centrale for udarbejdelsen af selvbetjeningsløsninger.

## Executive summary

This document outlines and explains a reference architecture for digital self-services for all of the Danish public sector: municipalities, regions, state agencies and ministries. This reference architecture is part of the implementation of the initiatives in the joint public digitization strategies. The reference architecture has been produced by a group of IT-architects and other experts from a number of public authorities. This version will be updated as experience is gathered through the coming use of the reference architecture.

The purpose of the reference architecture is to target the efforts in the public sector on producing interconnected, efficient, secure and useable self-services to citizens and enterprises, as well as to generate financial benefits for public authorities, e.g. through decreased need for support calls and improved interconnectivity between self-service solutions from various and diverse authorities. The reference architecture is intended to establish a common understanding of the business and it-architecture of self-services across the public sector, and between public authorities and their suppliers. In this document “self-service” means digital self-service with a focus on interactive internet-based communication.

Government digital self-service has traditionally focused on the collection of data for the execution of statutory tasks of the respective authorities, often with a functionality based fairly closely on the paper forms from which the self-service systems are often based upon. However, in recent years the public sector in Denmark has invested in increasingly user-friendly and efficient self-service systems as a part of the implementation of legislation making it mandatory for citizens and companies to use a range of self-services for applications, filings, etc. The further development of self-service systems  will require a focus on creating a more coherent user experience, especially in situations where the user use more than one self-service system to perform his or her task. In addition, self-service systems will have to be designed to support a larger part of the overall tasks the user has beyond the basic data capture.

The purpose of this reference architecture is to create a framework for facilitating increased user satisfaction and greater efficiency in the overall execution of the tasks involved when citizens or companies interact with government online. This includes better support for the tasks and needs of the user, more reuse of data and better integration with back-office systems and processes. It includes better coherence and collaboration between various and diverse self-service systems when the user needs to use more than one system to solve his or her task and needs. And it is likely to include a higher degree of automation to allow parts of the process, in some cases the entire process, to run without manual processing, resulting in faster – sometimes immediate – decisions.

This reference architecture renders the perspective of the user (methodically: the user journey) the framework for the design of a self-service process. This includes supporting the initial introduction to the task and clarification of the context, a flexible and user-friendly completion of the task and the provision of clear information about what happens after the self-service is finished.

In this reference architecture, the user journey is construed as the user’s experience of a self-service process or a chain of self-service processes, and the term is thus used in a narrower sense than its standard conceptualization in UX design.

Seen from an authority or an architectural perspective, a self-service process consists of a preparation, a completion of the core self-service process and a round-off of the process. The purpose of the preparation is to assist the user in understanding the task ahead, the tasks he or she will have to prepare for (like gathering documentation and information) and to clarify the context in order to help the user determine whether the present self-service process makes sense, given the users situation and needs. The core is where the data capture takes place and where the user can read and accept the terms and conditions that apply to the application, filing, etc. involved. The round-off is intended to ensure that the user understands what the completion of the core and the submission of the information entail, what happens next and what further opportunities or obligations the new context might give the user.

Furthermore, the reference architecture describes a framework for how a user journey comprised of several self-service processes can be combined into self-service chains. This chaining is achieved through a handover, and the reference architecture includes provisions to ensure that such handovers can take place between different authorities.

The reference architecture for self-service initiate a set of principles for establishing a common IT architecture for self-service systems, but is based on the Danish federal digitalization arkitecture principles, here architecture rule 2.4 "Build change-ready solutions with the user as its starting point" and 5.1 "Design coherent user journeys".

Self-service principles

1. In a self-service process, the user encounters preparation, core and round-off, supported by user-focused digital systems.
2. Self-service systems are comprehensible, easy and intuitive to use for the intended users.
3. The user only has to provide information the government does not already have.
4. The user meets a coherent and interconnected service, even when it crosses sectorial boundaries of different authorities.
5. It is always clear for the user which authority is responsible for a given service or part of a service.
6. Authorities involved in the chaining of several self-service processes, establish agreements on the division of tasks and responsibilities, within the current rules and regulations.

The core services realise the following capabilities in the reference architecture:

* Preparation
* Core
* Round-off
* Handover (from one self-service process to the next)

Combined, these capabilities realise a self-service process and are used by citizens or staff in companies. They may be initiated by the users themselves or automatically, e.g. by back-office systems. The capabilities draw on a number of functionalities described in this document and establish and maintain a self-service context, making it possible for a self-service process to be put on hold and resumed. In case a handover is necessary, it is described which agreements will have to be made for this to take place. The capabilities may draw on information from back-office systems, from user profiles and from joint public infrastructure such as basic data, user management systems (identity and login), etc. See figure 5. Capabilities and actors in self-service processes/self-service chains.

The reference architecture shows what software components are used in the construction of self-service systems and which joint public infrastructure components the self-service systems will draw on. See figure 16. Possible components in self-services. The reference architecture lists the software technologies available in the market for the construction of self-service systems.

The reference architecture sets requirements for the common public infrastructure components and also proposes new ones. The reference architecture points out which existing standards to use and new standards to be developed. The reference architecture touch upon the security issues which are central for the design and implementation of self-service systems.

## Indledning

### Formål

Denne referencearkitektur er udarbejdet i sammenhæng med den fællesoffentlige arkitektur for digitalisering (FDA) og er en del af den fælles rammearkitektur, der skal understøtte implementeringen af de fællesoffentlige digitaliseringsstrategier. Formålet er, at referencearkitekturen skal fungere som basis for en fælles forståelse af forretningsarkitekturen, herunder de forvaltningsmæssige processer og begreber. Det vil sige fælles begreber for digital selvbetjening, der understøtter bedre dialog mellem myndigheder, herunder myndigheder, der varetager infrastrukturkomponenter i portaler - og i forhold til leverandører i anskaffelsesprocesser. Derudover også som et teknisk pejlemærke for udvikling af digitale løsninger generelt i den offentlige sektor, herunder for udvikling af fælles standarder og løsninger.  
   
Referencearkitekturen skal understøtte udviklingen af bedre selvbetjeningsløsninger. Formålet er at kunne give brugerne en vellykket brugeroplevelse, således at de kan gennemføre selvbetjeningsforløb med et minimum behov af support fra de involverede myndigheder, herunder suppoort via andre kanaler.

Denne referencearkitektur vil derfor løfte brugeroplevelsen i selvbetjening generelt ved at:

* Gøre brugerrejser til den centrale forståelsesramme for tilrettelæggelse af selvbetjeningsforløb med udgangspunkt i den eller de opgaver, som en bruger skal have løst.
* Tænke forberedelse, kerne, genoptagelse og afrunding ind i selvbetjeningsforløbet.
* Anvende allerede kendte data om brugerne, hvor de er tilgængelige.

Referencearkitekturen skal desuden give mulighed for at styrke den tværgående sammenhæng i de offentlige selvbetjeninger ved hjælp af overdragelse:

* I selvbetjeningsforløbet overføres status og procesdata, som bruges til at skabe sammenhæng på tværs. 
* Der skabes ramme og instrumenter til at kæde selvbetjeningsforløb sammen på tværs af ministerområder og ressortområder.

Med henblik på at understøtte dette vil denne referencearkitektur derfor:

* Præsentere en fælles forståelse af selvbetjening, herunder beskrivelse, definition, sprog og scope for selvbetjening.
* Give retningspile til de mange forskellige teknologier, som kan realisere selvbetjening som sammenhængende brugerrejser både som enkelte selvbetjeningsforløb og som selvbetjeningskæder.

Referencearkitekturen bygger på mange års erfaringer med selvbetjeningsløsninger til browsere på pc’er, tablets og smartphones og til apps. Udviklingen i teknologier og brugerforventninger betyder, at referencearkitekturen er et bedste bud på en sammenhængende arkitektur for området og det forventes, at den løbende udvikles. Der må påregnes justeringer af referencearkitekturen efter de forretningsmæssige erfaringer, der kommer fra portaler som virk.dk og borger.dk, samt fra initiativerne i de fællesoffentlige digitaliseringsstrategier.

### Publicering og relaterede dokumenter

Referencearkitekturen publiceres på arkitektur.digst.dk, hvor man kan finde yderligere information om relaterede emner og beslægtet information om rammearkitektur, øvrige referencearkitekturer, byggeblokke, standarder, krav, metoder, styring mv.

### Målgruppe

Den primære målgruppe for dette dokument er arkitekter, tilknyttet offentlige digitaliseringsprojekter, herunder enterprise-arkitekter, forretningsarkitekter, løsningsarkitekter, it-arkitekter mv. 

Dokumentets Del A Strategi henvender sig desuden også til projektledere og beslutningstagere, herunder forretningsansvarlige, digitaliseringschefer, it-chefer, afdelings- og kontorchefer - og andre med rollen som systemejer. 

Andre målgrupper for denne referencearkitektur er offentlige tjenesteudbydere og indirekte deres leverandører. Det anbefales at de sætter sig grundigt ind i referencearkitekturen.

### Anvendelse

Referencearkitekturen har overordnet set to anvendelseskontekster: Standardiseringsprojekter, der skal identificere, udvælge og eventuelt udarbejde fælles standarder, samt løsningsprojekter, der har til opgave at udvikle selvbetjeningsløsninger.

I forhold til standardiseringsprojekter anvendes referencearkitekturen til at udpege standarder, der understøtter skabelsen af sammenhængende, effektive, sikre og brugervenlige løsninger på tværs af sektorer, nationalt og transnationalt. Referencearkitekturen fokuserer på at rammesætte, kravsætte og vejlede fællesoffentlige selvbetjeningsløsninger, domæneløsninger og enkelte myndigheders selvbetjeningsløsninger.

I forhold til løsningsprojekter anvendes referencearkitekturen i forbindelse med konceptualisering af løsningsarkitektur og kravspecificering. Den kan fx også anvendes i forbindelse med specificering af standardiserede snitflader mellem systemer, der skal kunne arbejde sammen, for så vidt at løsningen indeholder komponenter og services, der er omfattet af referencearkitekturen. Referencearkitekturen anviser ikke i detaljer, hvordan løsninger skal bygges, men fastlægger overordnede rammer og peger på områder for fælles standarder for løsninger.

Referencearkitekturen definerer, hvad en sammenhængende løsning omhandler i rammerne af dens emne, og den beskriver de udfordringer, der skal håndteres for at skabe sammenhængende løsninger. 

Referencearkitekturen kan anvendes i sammenhæng med andre fællesoffentlige referencearkitekturer, der behandler relaterede udfordringer.

Generelt kan en referencearkitekturs rolle illustreres ved følgende figur:

![Figur 1.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%201.jpg)

Figur 1. Referencearkitekturens rolle

### Krav til overholdelse af referencearkitekturen

Bilag A Tjekliste indeholder en oversigt over en række af de mest centrale dele af referencearkitekturen, som man skal være opmærksom på i et projekt, der har et scope, hvor denne referencearkitektur kan være relevant.

Referencearkitekturen er som del af den fællesoffentlige rammearkitektur styrende for arkitekturarbejdet i projekter i den fællesoffentlige digitaliseringsstrategi. Dette omfatter dels løsningsprojekter vedrørende fællesoffentlige komponenter og services i form af infrastrukturløsninger som fx borger.dk og virk.dk, Digital Post, MitID og NemLog-in, dels projekter, der indebærer, at myndigheders løsninger skal kunne arbejde sammen og dele data. Desuden er referencearkitekturen styrende for det fællesoffentlige arbejde med at udvikle fælles standarder i regi af strategien.

I forbindelse med projekter, som indgår i den fællesoffentlige digitaliseringsstrategi, er der aftalt en governance-ramme. Denne omfatter en række fora, herunder Udvalget for Arkitektur og Standarder (UAS), der har ansvar for de referencearkitekturer og standarder, som optages i den fællesoffentlige digitale arkitektur (FDA). UAS håndhæver governance gennem review af projekter, som foretages af et fællesoffentligt reviewboard.

På hjemmesiden arkitektur.digst.dk kan man læse nærmere om rammerne for governance vedrørende den fællesoffentlige rammearkitektur, herunder konkrete aftaler og beslutninger vedrørende anvendelse og realisering af nærværende referencearkitektur. Derudover kan referencearkitekturen frit anvendes som vejledende teknisk pejlemærke.

### Kontekst for tilblivelse og styring

Referencearkitekturen er udarbejdet i dialog med en arbejdsgruppe bestående af deltagere fra Digitaliseringsstyrelsen, Erhvervsstyrelsen, SKAT, KL, Landbrugs- og Fiskeristyrelsen (senere Landbrugsstyrelsen), Miljøstyrelsen og ATP og gennem møder med arbejdsgruppen for rammearkitektur og referencearkitekturer og i samarbejde med arbejdsgruppen for selvbetjening. 

Referencearkitekturens er optaget i den fællesoffentlige rammearkitektur ved godkendelse på et møde UAS. Forud for dette har dokumentet gennemgået mindst ét review af et review board, nedsat af UAS og har deltaget i en åben ekstern kommentering, med inddragelse af relevante interessenter, herunder en bred kreds af myndigheder og leverandører.

### Definitioner og begreber

Kapitel 9 Begrebsmodel beskriver den centrale begrebsmodel for referencearkitekturens domæne. Denne begrebsmodel har været underkastet review af Styregruppen for data og arkitektur.

Bilag B indeholder en samlet ordliste over referencearkitekturens begreber og terminologi. 

Væsentlige begreber forklares undervejs.

### Anvendt metode og notation

Referencearkitekturen følger den fælles rammearkitekturs metoder og er udarbejdet efter en vejledning og skabelon for referencearkitekturer, version 0.3 august 2017. Anvendte notationer omfatter Archimate, UML og BPMN.

Referencearkitekturen er generelt søgt udarbejdet således, at den er så konsistent som muligt med øvrige arkitekturdokumenter og standarder, udarbejdet i regi af den fællesoffentlige rammearkitektur.

Referencearkitekturen bygger på etablerede fællesoffentlige arkitekturprincipper, aftaler og retningslinjer vedrørende arkitektur, data og anvendelse af åbne standarder. 

Fremtidige revisioner af denne referencearkitektur vil blive tilpasset revisioner af rammearkitekturen, herunder metoderammer og relaterede referencearkitekturer.

### Sammenhæng til den fællesoffentlige rammearkitektur

Denne referencearkitektur er del af den samlede fællesoffentlige digitale arkitektur, FDA-rammearkitektur. FDA-rammearkitektur udfoldes i en række referencearkitekturer, som hver dækker et emnefelt og gensidigt supplerer hinanden. I første omgang omfatter det emnerne brugerstyring, deling af data og dokumenter samt tværgående digitalt overblik for borgere og virksomheder (i relation til digital selvbetjening).

For en introduktion til og overblik over den samlede rammearkitektur samt relateret information henvises til arkitektur.digst.dk/rammearkitektur.

Referencearkitektur for selvbetjening bygger bl.a. på komponenter og andet, der behandles og beskrives detaljeret i disse referencearkitekturer. Det gælder fx samtykke og fuldmagt. Det gælder adgang til data, hvor referencearkitekturen forudsætter, at brugerens data hentes ved kilden, når det skal udstilles for brugeren. 

### Læsevejledning

* Del A Strategi bør læses af alle. Omfatter en introduktion til emnet, de overordnede styringsrammer, forretningsmæssige behov, vision, forretningsmæssigt målbillede og værdiskabelse. Giver et kort overblik over as-is situationen, gap og forudsætninger samt overvejelser om migration frem mod målbilledet. Desuden beskriver denne del de juridiske og sikkerhedsmæssige bindinger samt de overordnede principper, som sætter rammer for digitale selvbetjeningsløsninger.
* Del B henvender sig særligt til forretningsarkitekter. Her beskrives de grundlæggende begreber og det organisatoriske perspektiv med fokus på de forretningsmæssige kapabiliteter og processer.
* Del C henvender sig særligt til løsningsarkitekter. I denne del beskrives de væsentligste tekniske applikations- og infrastrukturkomponenter, herunder services og integrationer samt områder for fælles tekniske standarder. Endvidere beskrives overordnet, hvordan komponenterne kan realiseres.
* Bilagene omfatter en tjekliste, som kan anvendes af projekter til at få overblik over de vigtigste spørgsmål, som man skal forholde sig til i relation denne referencearkitektur. Desuden er der i Bilag B en samlet ordliste med anvendte begreber og termer samt en kildefortegnelse. 

## Del A Strategi

### Introduktion

#### Beskrivelse af emnet selvbetjening

Med selvbetjening menes i dette dokument digital selvbetjening med fokus på interaktiv, internetbaseret kommunikation.

Det offentlige Danmark har i de seneste år investeret i mere brugervenlige og effektive selvbetjeningsløsninger som led i udmøntningen af lovgivning af obligatorisk digital selvbetjening (bølgeplanerne) og har flyttet en stor del af henvendelserne til myndighederne over på de digitale løsninger. På trods af dette fremstår mange digitale løsninger isolerede i forhold til at skabe sammenhæng for brugeren i de situationer, hvor løsningen af brugerens opgave kræver anvendelse af flere selvbetjeningsløsninger. Løsningerne har dog i højere grad understøttet de øvrige opgaver, borgeren eller virksomheden måtte have i forbindelse med den opgave, selvbetjeningen indgår i. Fokus er derfor stadig, at brugerne (borgere og virksomheder) oplever sammenhæng på tværs af løsninger, samtidigt med at kvaliteten af den enkelte løsning er høj.

Flere forhold vil kunne bidrage både til en større brugertilfredshed og til en større effektivitet i den samlede opgaveløsning. Det er forhold, som udgør fx en højere grad af understøttelse af borgerens eller virksomhedens samlede opgave og behov, en højere grad af genbrug og en mere effektiv validering af data og en bedre integration til fagsystemer m.m. samt en bedre sammenhæng mellem løsningerne, når brugeren skal anvende flere ad gangen. Dette kan blandt andet ske ved at gøre det muligt at øge automatiseringsgraden, så en større del af processen – og på nogle områder hele processen – kan gennemføres uden at involvere en sagsbehandler og derved evt. resultere i straksafgørelser.

Endelig giver udviklingen i og udbredelsen af mobile enheder (devices, apparater) mulighed for nye former for interaktivitet og mulighed for at udvide antallet af selvbetjeningskanaler.

Der er i de senere år flere steder i offentlige projekter blevet sat fokus på at tilrettelægge selvbetjening ud fra et fokus på brugerens oplevelse fremfor alene at tænke ud fra forvaltningens perspektiv. Disse digitale løsninger har understøttet borgere og virksomheders proces, ligesom de har effektiviseret myndighedernes processer. Denne referencearkitektur gør brugerrejsen til en ramme for tilrettelæggelse af selvbetjening, hvor perspektivet er at levere en mere sammenhængende understøttelse af brugerrejsen ved, som en del af selvbetjeningsforløbet, at indføre brugeren i den opgave, der skal løses med selvbetjening, understøtte smidig og brugervenlig løsning af opgaven og afslutte med klar besked om, hvad der derefter skal ske, og evt. hvilke videre muligheder brugeren har. 

Med arkitektens perspektiv beskrives det som et selvbetjeningsforløb med forberedelse af brugeren, gennemførelse af kernen i selvbetjeningsforløbet og afrunding af selvbetjeningsforløbet. Forberedelse skal afklare og styrke brugerens forståelse af den opgave, der skal løses. Kernen er der, hvor opgaven løses, såsom at læse og godkende, ansøge, indberette og lign. Afrunding skal sikre, at brugeren er klar over, hvad gennemførelsen af kernen har bibragt brugeren, og hvilke muligheder denne nye kontekst har for brugeren. 

Referencearkitekturen beskriver desuden rammerne for, at brugerrejser, der omfatter flere selvbetjeningsforløb, kan kædes sammen i selvbetjeningskæder med efterfølgende større brugertilfredshed. Selvbetjeningsforløb kædes sammen gennem overdragelse, og referencearkitekturen tager højde for, at overdragelse kan ske mellem forskellige ressortområder.

![Figur 2.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%202.jpg)

Figur 2. Selvbetjeningsforløb

En selvbetjeningsløsning er følgelig den tekniske løsning, der implementerer et selvbetjeningsforløb og eventuel overdragelse til et efterfølgende selvbetjeningsforløb.

En bruger er her en person, der enten optræder som borger eller optræder i en rolle som repræsentant for en virksomhed. 

Et simpelt eksempel kunne være en borger, der gerne vil have hjælp til gratis befordring til behandling på sygehuset, som kunne forløbe som følger:

* I forberedelsen (som i dette eksempel sker, efter borgeren er logget på med sit NemID), afklares det, om borgeren som udgangspunkt tilhører en målgruppe, der har ret til gratis befordring eller til at få refunderet befordringsomkostningerne.
* En del af de nødvendige oplysninger (som fx om borgeren er pensionist, og hvor langt borgeren har til sygehuset) kan selvbetjeningsløsningen selv finde ved at slå op i relevante registre. Andre skal borgeren selv levere i selve kernen. 
* I slutningen af forberedelsen får borgeren at vide, om han falder inden for en af de grupper, der har mulighed for at få sine transportudgifter helt eller delvist dækket, hvor han skal søge, og hvilken dokumentation han evt. skal have klar. 
* Efter forberedelsen ledes borgeren til det relevante ansøgningsforløb (kernen), hvor han fx uploader dokumentation eller booker transport samt indtaster evt. øvrig påkrævet information. 
* I afrundingen får borgeren dels en kvittering for de oplysninger, han har sendt (ansøgning), dels besked om, hvad det videre forløb vil være (fx at han vil få en mail med nærmere oplysninger om transporten, eller hvornår han vil få refunderet sine udgifter). Desuden kan han få at vide, hvem han kan kontakte, hvis han har spørgsmål.

#### Brugerrejser, hvor der skal løses flere opgaver

Der findes rigtig mange brugerrejser, hvor der kun løses én opgave. Men der findes også brugerrejser, hvor der skal løses flere opgaver, og hvor borgeren eller virksomheden kan have en forventning om at blive hjulpet gennem alle opgaverne. Desuden stiller forvaltningsloven krav om vejledning, dvs. at myndigheden har pligt til at yde vejledning til borgerne for at hjælpe borgeren med at undgå fejl, og at de som følge af uvidenhed eller misforståelser udsættes for et retstab.

I brugerrejser, hvor der skal udføres flere opgaver i sammenhæng, er det myndighedernes opgave at skabe en brugeroplevelse, hvor brugeren ikke oplever ulemper som følge af, at de enkelte opgaver er fordelt på flere myndigheder og selvbetjeningsløsninger. Er der tale om løst koblede forløb, hvor sammenhængen fx skabes i forberedelsen og gennem en tjekliste med links, behøver der ikke at være nogen tidsmæssig begrænsning på forløbet. Er der tale om mere stramt koblede forløb med tættere sammenhæng mellem de enkelte trin i forløbet, kan det være relevant at synliggøre en evt. tidsgrænse for, hvornår næste skridt eller evt. hele forløbet skal være gennemført. Det indgår i tilrettelæggelsen af en selvbetjeningskæde at oplyse brugeren om, hvor lang tid han kan forvente at få en sammenhængende service.  
   
Eksempel på selvbetjeningskæde – selvbetjeningsforløb med flere opgaver  
Her følger et konstrueret (og forenklet) eksempel på en brugerrejse bestående af to selvbetjeningsforløb og dækkende flere opgaver med udgangspunkt i, at en borger ønsker at søge boligstøtte. 

Borgeren er meget fokuseret på, at han kan få boligstøtte til en ny bolig og går i gang med ansøgningsforløbet, selv om han ikke har meldt flytning til folkeregisteret endnu. I forberedelsen (1) til boligstøtte afdækkes konteksten for boligstøtteansøgningen gennem et interaktivt spørgsmål/svar-forløb: Hvad er baggrunden? Er der sket ændringer i borgerens indkomst eller husstandsforhold, eller skal borgeren flytte til en ny bolig? Eksemplet tager udgangspunkt i, at borgeren er enlig og flytter til en ny lejebolig, hvor han også vil være enlig. Forberedelsen munder ud i, at borgeren får at vide, at han skal melde flytning til den nye adresse, før han kan søge boligstøtte. 

Fra forberedelse i boligstøtteløsningen kan borgeren så gå videre til flytteløsningens forberedelse (3). Dette sker gennem en overdragelse (2). Flytteløsningen kan nu i sin forberedelse trække på de oplysninger, borgeren har givet i boligstøtteløsningens afklaring. Den kan også anvende oplysningerne til at forudfylde relevante dele af flytteanmeldelsen (kernen (4)) med de oplysninger, der er givet. Når kernen afsluttes, får borgeren som en del af afrundingen (5) at vide, at en kvittering er sendt til vedkommendes digitale postkasse. 

I dette tilfælde kan flytningen gennemføres som en straksafgørelse. Borgeren får derfor også som en del af afrundingen at vide, at han (gennem en overdragelse (6)) kan vende tilbage til boligstøtteansøgningen og færdiggøre denne. 

![Figur 3.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%203.jpg)

Figur 3. Selvbetjeningskæde med to sammenkædede selvbetjeningsforløb, der løser hver sin opgave

Gennem tilrettelæggelse af selvbetjeningsforløbet ud fra brugerens oplevelse sættes der fokus på brugerens behov i såvel forberedelse, kernens gennemførelse, afrunding og eventuelle overdragelse. Dermed skabes der mulighed for, at brugeren i højere grad lykkes med at anvende selvbetjening og udføre tingene i den rette rækkefølge, så det i mindre grad er nødvendigt for brugeren at kontakte myndigheden eller for myndigheden at kontakte brugeren som følge af komplikationer i forløbet. 

#### Styringsrammer

Digitale selvbetjeningsløsninger er styringsmæssigt forankret hos den myndighed, der har ansvaret for at levere den pågældende myndighedsopgave/service til borger og virksomhed. Af hensyn til borgeres og virksomheders brugeroplevelse og sammenhæng i det offentliges selvbetjeningsløsninger er der etableret en række fællesoffentlige løsninger, standarder og vejledninger, der styres af de samarbejds- og styringsorganer, der er etableret senest i forbindelse med den fællesoffentlige digitaliseringsstrategi 2016-2020. Denne referencearkitektur er en del af dette fællesoffentlige samarbejde.

Løsningsmæssigt kan selvbetjeningsløsninger tilgås fra myndighedens hjemmesider og fra de tre fællesoffentlige portaler: borger.dk, virk.dk og sundhed.dk. Herfra skal der, via de fællesoffentlige aftaler, også være adgang til myndighedernes selvbetjeningsløsninger. Det er ligeledes aftalt, at offentlige hjemmesider og selvbetjeningsløsninger med behov for sikkert login og rettighedsstyring anvender de fællesoffentlige løsninger til brugerstyring.

Digitaliseringsstyrelsen udarbejder løbende vejledninger til gode selvbetjeningsløsninger. Disse findes på Digitaliseringsstyrelsens hjemmeside.

Der er ikke etableret yderligere styringsmæssige rammer for selvbetjeningsløsninger, der indgår i selvbetjeningskæder på tværs af myndigheder. Det må aftales mellem de involverede myndigheder i hvert enkelt tilfælde gennem en overdragelsesaftale, som sikrer, at alle forhold er afklaret mellem myndighederne med hensyn til overdragelse af data, kvaliteten af disse data og transporten af dem. Dette redegøres der nærmere for i [afsnittet om forretningskapabiliteter](/node/1100#forretningskapabiliteter).

### Vision, scope og mål

#### Forretningsmæssige behov (drivere)

Der er i forhold til de offentlige selvbetjeningsforløb forsat et potentiale for forbedringer af brugeroplevelsen og for at udvikle selvbetjeningsløsningerne, så de i endnu højere grad kan bidrage til effektiviteten og kvaliteten i sagsbehandlingen. Det gælder både i forhold til løsningerne set enkeltvis og i forhold til forløb, hvor brugeren skal anvende flere forskellige løsninger for at løse sin opgave, og som evt. går på tværs af myndigheds- og forvaltningsområder. 

Referencearkitekturen skal bidrage til, at dette potentiale i højere grad kan realiseres, bl.a. ved at understøtte etableringen af selvbetjeningsforløb, der omfatter en større del af brugerens opgave, såvel som brugerrejser, der omfatter flere selvbetjeningsforløb og/eller går på tværs af myndigheds- og ressortgrænser.

Referencearkitekturen skal være en hjælp til og udgøre en ramme for de enkelte myndigheder i udviklingen af selvbetjeningsløsninger og i dialogen med leverandører, herunder understøtte kravspecificering i forbindelse med udbud og indkøb. Referencearkitekturen vil også skulle være en støtte for de leverandører, som ønsker at sikre sig, at de løsninger, som de selv udvikler, er i overensstemmelse med referencearkitekturen, og at de anvender sprog og begreber som defineret i referencearkitekturen. Der vil dog være behov for at udarbejde vejledninger, bidrag til kravspecifikationer og anden bistand på en række områder.

#### Vision

Afsættet for denne referencearkitektur er den fællesoffentlige digitaliseringsstrategi 2016-2020, som satte kursen for den fællesoffentlige digitalisering og samspillet med erhvervslivet. Referencearkitektur for selvbetjening skal bidrage til at nå digitaliseringsstrategiens mål om, at det digitale skal være let, hurtigt og sikre god kvalitet.

**Vision**  
Borgere og virksomheder oplever – når de skal løse opgaver digitalt i selvbetjeningsløsninger – at de kan gøre det let, hurtigt og overskueligt, også når deres brugerrejse inkluderer flere selvbetjeningsløsninger. De offentlige selvbetjeningsløsninger er indrettet med udgangspunkt i brugernes behov og skaber således sammenhæng, tryghed og sikkerhed for borgere og virksomheder, også når de går på tværs af myndigheds- og sektorgrænser.

En gennemførelse af referencearkitekturens anbefalinger vil medføre, at borgere og virksomheder i højere grad end i dag kan betjene sig selv digitalt i forhold til det offentlige på både en tryg og effektiv måde. Myndighederne vil modtage data, der er mere korrekte og komplette, der vil færre tilbageløb i processerne og mulighed for en højere grad af automatisering. Brugerne skal have mulighed for at vælge og skifte kanal efter behov. Resultatet vil være større brugertilfredshed, mere effektive processer og en højere kvalitet i data og i sagsbehandlingen.

##### Scope for arkitekturen

Inden for scope er:

* Vejledning af myndighederne om vellykket forberedelse, gennemførelse af kernen, afrunding af selvbetjeningsforløb og overdragelse.
* At understøtte, at et antal selvbetjeningsforløb på tværs af myndigheder eller afdelinger kan sammenkædes vellykket, set fra borger eller virksomhed, så længe at langt hovedparten af aktiviteterne gennemføres ved brug af digitale kanaler og værktøjer.

Uden for scope er:

* Den del af myndighedens sagsbehandling, der ikke direkte involverer borgerne eller virksomhederne.
* Brugerrejser, hvori der indgår fysiske møder, behandlinger eller vurderinger. Disse betegnes som tværgående procesforløb. I sådanne forløb kan dog nogle trin bestå af selvbetjeningsforløb, der løses indenfor rammerne af denne referencearkitektur. 
* Fuldt maskinel indberetning mv. er ikke omfattet af denne referencearkitektur, fx indberetning til SKAT af løn eller overførsel af data fra blodtryksmålere eller fra en bil til offentlige løsninger. Såfremt sådanne indberetninger kræver bekræftelse, visning af status eller anden opfølgning, vil det være omfattet af denne referencearkitektur.

#### 

As-is situationen

Med indførelse af obligatorisk selvbetjening på en række områder er en stor del af borgernes og virksomhedernes indrapportering af data til ansøgninger, løbende sager,  m.m. blevet digitale. Det har bidraget til at sikre Danmarks førerposition, når det drejer sig om digital kommunikation mellem borgere og virksomheder og myndighederne.

Der er i de fællesoffentlige digitaliseringsstrategier øget fokus på at understøtte den brugerrejse, som en bruger skal igennem ved benyttelse af offentlig selvbetjening. Det kræver vejledning til brugerne, før de går i gang med at indberette data, eller vejledning om det videre forløb og eventuelle nye muligheder, som brugerne kan have brug for efterfølgende. Ved brugerrejser, der indebærer anvendelse af flere selvbetjeningsforløb og som evt. krydser myndigheds- eller ressortområder, skal det i mindre omfang være overladt til brugeren selv at skabe den nødvendige helhed, sammenhæng og overblik. De videre forløb og eventuelle nye muligheder skal knyttes bedre sammen af myndighederne, både forretningsmæssigt og teknologisk. 

Brugeren er også i nogle tilfælde nødt til at indtaste data, vedkommende allerede har afleveret én gang til det offentlige. Det sker pga. manglende genbrug af data og løsningerne udnytter ikke altid fuldt ud de muligheder, der er, for at validere de data, der afleveres - og dermed sikre, at de er så komplette og fejlfrie som mulig.

Der arbejdes mange steder i det offentlige på at løse disse udfordringer. Flere steder er der interaktive selvbetjeningsforløb, der afleverer data dybt ind i fagsystemer. Der findes også nogle få selvbetjeningsforløb, der er koblet sammen med andre selvbetjeningsforløb. Hertil kommer, at portalerne bidrager til at skabe sammenhæng for brugerne.

Hensigten med denne referencearkitektur er at understøtte og lette dette arbejde.

#### Forretningsmæssigt målbillede (to-be situation)

De forretningsstrategiske mål med referencearkitekturen er:

1\. Øget brugervenlighed og øget selvhjulpenhed  
Det skal være lettere for borgere og virksomheder at betjene sig selv, også på tværs af myndigheds- og sektorgrænser og på deres foretrukne platforme, og de skal i højere grad opleve at kunne klare opgaven trygt og kompetent uden behov for supplerende kontakt til myndighederne.

2\. Nemmere afklaring hos myndigheder og leverandører  
Myndigheder og leverandører skal have et fælles sprog i forhold til selvbetjening, det skal være enklere for myndighederne at beskrive kravene til selvbetjeningsløsninger, hurtigere at udvikle nye løsninger og at implementere løsninger på nye kanaler.

3\. Bedre brug af data  
Det skal være mere transparent for brugerne, hvad data bruges til og af hvem, og løsningerne skal i højere grad genbruge data, myndighederne allerede er i besiddelse af. I de situationer, hvor behandling af data kræver samtykke, skal det være mere transparent, hvad brugerne giver samtykke til.

4\. Mere effektive processer  
Løsningerne skal medvirke til en højere kvalitet af de data, der indberettes, og dermed sikre færre tilbageløb, større muligheder for (hel eller delvis) automatisering og mere effektive processer.


#### Værdiskabelse

De målbare gevinster, disse strategiske mål skal tilvejebringe, er oplistet her. Realiseringen af referencearkitekturen vil skabe værdiværdi på følgende områder:

##### 1\. Flere vellykkede brugerrejser

En højere grad af understøttelse af brugernes samlede opgave antages at føre til øget brugertilfredshed.

Når brugerne i højere grad tages ved hånden (ved at det enkelte selvbetjeningsforløb introduceres gennem forberedelse, understøtter brugeren i gennemførelse af kernen og hjælper brugeren videre gennem afrunding), når data i større omfang genbruges og valideres bedre, og når sagsbehandlingstiden bliver kortere, antages det, at flere brugere ender med en vellykket brugerrejse, der opfylder de mål, vedkommende havde med rejsen.

Den samlede brugertilfredshed med selvbetjeningsløsningerne kan måles med de redskaber og metoder, der identificeres i projektet ”Viden om brugernes anvendelse af digitale selvbetjeningsløsninger” i regi af den fællesoffentlige digitaliseringsstrategi (2016-2020).

##### 2\. Reduceret behov for kontakt på andre kanaler i forbindelse med selvbetjening

Når brugerne i højere grad bliver hjulpet i vejen ind og ud ad løsningen, i forståelsen af den efterfølgende proces og i datavalideringen af de oplysninger, de afleverer, antages det, at behovet for kontakt på andre kanaler undervejs i forløbet reduceres. Det gælder i forhold til kontakter, initieret af brugeren (hvis vedkommende har behov for hjælp eller tryghed i processen), det gælder kontakter, initieret af myndigheden (hvis der er fejl eller mangler i de indsendte data/dokumentation), og det gælder til dels også afslag (hvis brugeren slet ikke er berettiget til det ansøgte eller evt. skulle have foretaget sig noget andet først).

Dette kan måles ved at tælle, hvor mange henvendelser myndigheden selv tager initiativ til og hvormange som skyldes mangler set fra brugerens synspunkt.

##### 3\. Løsninger, der er hurtigere at udvikle og vedligeholde

Når myndighederne kan tage udgangspunkt i en veldefineret arkitektur og i fællesoffentlige komponenter og vejledninger, som udvikles som en udmøntning af referencearkitekturen, antages det, at arbejdet med at kravspecificere nye løsninger bliver enklere, og at kommunikationen med leverandører bliver forbedret. Dette kan på længere sigt lede til, at det bliver lettere og hurtigere for leverandørerne at udvikle og vedligeholde løsningerne, og kunne føre til, at en del løsninger bliver billigere at anskaffe. 

Dette kan måles gennem en kvalitativ evaluering med inddragelse af leverandører og myndigheder.

##### 4\. Højere kvalitet i de data, der indrapporteres gennem løsningerne

Større genbrug af data, bedre understøttelse af brugeren i at finde data og bedre datavalidering vil betyde, at de data, der indrapporteres via løsningerne, i højere grad er fyldestgørende og korrekte. Det vil betyde færre tilbageløb i processen og bidrage til en hurtigere og mere effektiv sagsbehandling.

Dette kan måles ved tælle antal tilbageløb på grund af fejl i data i udvalgte sagsbehandlingsprocesser.

##### 5\. Øget automatiseringsgrad i processerne

En højere kvalitet i data og mere komplette data kan gøre det muligt i højere grad at automatisere hele eller dele af sagsbehandlingen. Dette vil mere effektivt understøtte såvel selvbetjeningsforløb som de dele af sagsbehandlingen, der kræver faglige vurderinger og skøn. Dette bidrager igen til kortere sagsbehandlingstider, hurtigere afgørelser og lavere omkostninger for myndighederne.

Dette kan måles ved at analysere udvalgte løsningers automatiseringsgrad.

#### Gap og forudsætninger

Realiseringen af disse mål og gevinster beror på en række forudsætninger:

##### 1\. Incitamenter

At der kan etableres de nødvendige incitamenter. Det omfatter incitamenter til at anvende arkitekturen (positive og negative), herunder at man finder en balance i hensynet til brugerne, den økonomiske business case og incitamenter til at producere gode fælles data og dele dem.

##### 2\. Kompetencer

At de nødvendige kompetencer til at anvende arkitekturen er til stede hos myndigheder og leverandører, herunder kompetencer til at tilrettelægge selvbetjeningsforløb ud fra brugerens oplevelse og tænke dem ind i en servicedesign -kontekst.

##### 3\. Lovgivning

At de nødvendige juridiske forudsætninger for deling af data og integration af forløb er på plads.

##### 4\. Governance

At der kan etableres den nødvendige governance i forhold til arkitekturen, herunder:

* Klare og forpligtende roller for aktørerne
* Klart ansvar for finansiering
* Sikring af, at arkitekturen vedligeholdes og videreudvikles 
* Sikring af en løbende kommunikationsindsats for arkitekturen.

##### 5\. Kritisk masse

At der kan opnås kritisk masse. Det vil sige, at arkitekturen anvendes som basis for udviklingen af nye løsninger i et omfang, der betyder, at der dannes et nyt paradigme for selvbetjeningsløsninger, der i højere grad understøtter vellykkede brugerrejser. Det nye paradigme supplerer ”blanket”-paradigmet, således at det bliver almindeligt, at der lægges lige stor vægt på forberedelse, kernen og afrunding, og at løsningerne er konstrueret til at indgå i sammenhængende forløb. Det kræver blandt andet:

* At arkitekturen og anvendelsen af den får en klar strategisk forankring.
* At aktørerne tager ejerskab til og bakker op om arkitekturen og dens formål, og den dermed bliver retningssættende for nye løsninger.
* At arkitekturen kan rumme, at forskellige domæner kan have forskellige behov og tilgange.
* At der kan opnås den nødvendige grad af interoperabilitet på tværs af myndigheder.
* At den nødvendige infrastruktur (herunder adgang til data) er på plads, og at der i tilstrækkeligt omfang udvikles fælles standarder, som får bred anvendelse.

En migration mod en implementering af det beskrevne målbillede kræver en indsats fra mange forskellige interessenter og omfatter derfor både implementering hos myndigheder som serviceudbydere.

Der udarbejdes derfor med en strategi for realisering, herunder et teknisk roadmap for fællesoffentlige standarder og komponenter samt styring og finansiering. Implementering af referencearkitekturen for selvbetjening sker i sammenhæng med andre tiltag under de fællesoffentlige digitaliseringsstrategier og under den styringsstruktur, som er nedsat til at realisere  indsatserne.

### Bindinger

I dette afsnit beskrives juridiske og sikkerhedsmæssige bindinger overordnet i forhold til selvbetjeningsløsninger. Detaljerede krav og løsninger er ikke del af denne referencearkitektur.

#### Jura

Borgeres og virksomheders brug af selvbetjeningsløsninger er omfattet af forvaltningsloven, persondataloven og lov om obligatorisk selvbetjening, EU’s databeskyttelsesforordning (persondataforordning) og af EU's webtilgængelighedsdirektiv. For selvbetjeningsløsninger, der kan anvendes af borgere fra EU/EØS-lande, vil eIDAS-forordningen også have betydning.

Mange selvbetjeningsløsninger er omfattet af lovgivningen om obligatorisk digital selvbetjening. Folketinget har vedtaget i alt fire samlelove  om obligatorisk digital selvbetjening, som danner grundlaget for obligatorisk digital selvbetjening for borgere og virksomheder på en række områder, og som udmøntes i ændringer i den konkret faglovgivning.

Desuden er selvbetjeningsløsninger omfattet af de pågældende myndigheders ressortlovgivning. Det betyder, at hver enkelt selvbetjeningsløsning skal være forankret hos en myndighed. Det betyder ligeledes, at myndigheder, der samarbejder om at kæde selvbetjeningsløsninger sammen, skal gøre det inden for rammerne af disse regler.

Inden for selvbetjening skal der være særligt fokus på beskyttelse af persondata og privatlivets fred, på korrekt implementering af love og betænkninger som selvbetjeningen vedrører, at vejledningspligten er opfyldt og på beskyttelse mod fjendtlig indtrængen via internet. 

Lovgivning og forordning stiller krav til sikkerhed i myndighedernes it-løsninger, hvilket kort opridses herunder.

#### Sikkerhed

Den enkelte myndighed er ansvarlig for sikkerheden i egne selvbetjeningsløsninger.

Arbejdet med sikkerhed kan med fordel bygge på koncepter og værktøjer for informationssikkerhedsstyring. 

Det er obligatorisk for statslige myndigheder at anvende ISO 27001 . KL anbefaler alle kommuner at anvende ISO-standarden med henblik på at få en fælles, høj sikkerhedsstandard i den offentlige sektor, mens regionerne vil udarbejde en fællesregional informationssikkerhedspolitik, baseret på ISO 27001.

For selvbetjeningsløsninger er det udgangspunktet, at myndighederne ud fra en risikovurdering selv skal beslutte deres sikkerhedsniveau, hvilket også ligger i rollen som dataansvarlig i persondataloven. En sådan risikovurdering kan med fordel tage udgangspunkt i metodikken, defineret i ISO/IEC 27005, og styringen af informationssikkerhed kan med fordel tage afsæt i ISO/IEC 27001-standarden.

I forhold til den enkelte selvbetjeningsløsning skal den ansvarlige myndighed vurdere sikkerheden ud fra en række vinkler, som omfatter jura, organisering, informationer og teknik. Der skal specielt være fokus på, at en overdragelse medfører, at forhold omkring en databehandleraftale skal afklares og aftales.

Selvbetjeningsløsninger indgår i samspil med brugernes udstyr, med andre tjenester og med infrastruktur, dvs. forhold der ikke er under den enkelte myndigheds kontrol. Det gælder også i de tilfælde, hvor en brugerrejse omfatter flere selvbetjeningsløsninger, som derfor skal fungere sammen, i et eller andet omfang (sammenkædning til selvbetjeningskæder).

Konsekvenserne af dette og af et mere tværgående fokus på at skabe sammenhæng er, at det er nødvendigt med fælles rammer for sikkerhed, der definerer roller og ansvar for de forskellige komponenter. Der er desuden behov for, at den enkelte myndighed i sin sikkerhedspolitik og risikostyring inddrager disse sikkerhedsmæssige forhold.

##### Love og regler

I arbejdet med selvbetjeningsløsninger skal der dels tages højde for den konkrete lovgivning på området, dels generelle lovgivningsmæssige krav til informationssikkerhed. I det følgende nævnes de love og regler, der er kendt i oktober 2017. De generelle krav i blandt andet persondataloven og databeskyttelsesforordningen til sikker behandling af persondata rammesætter løsningernes tilrettelæggelse, adgangssikkerhed og teknologianvendelse (fx privacy by design, hvad og hvordan der kan gives adgang fra smartphones). 

Kravene i persondataloven er uddybet i sikkerhedsbekendtgørelsen . Tilsvarende gælder for krav til sikkerhed i nationale politikker som National strategi for cyber- og informationssikkerhed  og Sikkerhedskrav i domæners digitale strategier. Endelig er Danmark fra september 2018 forpligtet til at anerkende nationale eID’er fra andre EU/EØS-lande, når en bruger ønsker at logge ind på en dansk selvbetjeningsløsning. 

Digitaliseringsstyrelsen og Justitsministeriet vejleder om de generelle love, regler mv., der skal indgå i arbejdet med informationssikkerhed .

Den ansvarlige myndighed for selvbetjeningsløsningen skal desuden afdække de krav, som den konkrete lovgivning på området stiller til selvbetjeningsløsningen, fx hvilke informationer der skal/ikke skal behandles, og hvilke informationer der må hentes fra og leveres til andre myndigheder. Denne afdækning kan blandt andet omfatte, om der skal indhentes samtykke til udveksling af information, samt at der kun hentes den information, som forvaltning af selvbetjeningsforløbets opgave har brug for.

##### Organisering

Den enkelte myndighed skal som ansvarlig for sine selvbetjeningsløsninger etablere de relevante sikkerhedspolitikker og følge op på dem gennem fx overvågning, kontrol af logfiler og eventuel efterforskning af brud på sikkerheden. Såfremt driften af selvbetjeningsløsningen skal outsources, skal der hentes vejledning til at styrke sikkerheden i en rapport udarbejdet af Digitaliseringsstyrelsen og Center for Cybersikkerhed, der beskriver elleve konkrete anbefalinger til, hvordan sikkerheden i den outsourcede it-drift kan forbedres . I forbindelse med outsourcing skal der i henhold til sikkerhedsbekendtgørelsen udarbejdes en databehandleraftale.

##### Informationer

Analyse af informationssikkerheden bør omfatte en analyse af de informationer (data), der skal behandles i løsningen, hvilken grad af fortrolighed og følsomhed de har, og hvordan fortrolighed og integritet sikres bedst muligt.

Som en del af analysen af information bør der gennemføres en konsekvensvurdering for privatlivets databeskyttelse (også kaldet Privacy Impact Assessment, PIA). For statslige myndigheder er denne konsekvensvurdering obligatorisk for projekter, der følger den fællesstatslige projekt- og programmodel. En skabelon til formålet kan findes på Digitaliseringsstyrelsens hjemmeside .  
   
Databeskyttelsesforordningen fra EU (GDPR) skærper og erstatter krav til indholdet af en sådan vurdering (DPIA - Artikel 35), samt hvornår Datatilsynet skal konsulteres. En sådan konsekvensanalyse kan identificere behov for yderligere sikkerhedsforanstaltninger, der skal implementeres i tjenesten.

Krav til sikker databehandling skal spille sammen med hensyn til brugervenlighed. Det kan betyde klassificering og segmentering af data, således at selvbetjeningsløsninger kan tilgås med forskellige sikringsniveauer (som der er standarder for i National Standard for Identiteters Sikringsniveauer, NSIS) og med forskellige grader af identitetsinformationer som fx anonymitet.

##### Teknik

Analyse af de tekniske forhold omfatter, hvordan løsningen teknisk set kan leve op til de stillede krav til fortrolighed, integritet, uafviselighed og tilgængelighed, og hvilke tekniske risici der skal imødegås i tilrettelæggelsen og driften af løsningen. Myndighedens krav til sikkerhed skal implementeres i de komponenter, der indgår i selvbetjeningsløsningen.

##### Interoperabilitet

Da selvbetjeningsløsninger udstilles på internettet og indgår i samspil med andre tjenester, er sikkerheden ikke kun afhængig af forhold i den enkelte myndighed, men afhænger også af den infrastruktur og de komponenter, der leveres af andre parter. Det gælder fx de fællesoffentlige komponenter til brugerstyring (nationalt eID , login, rettigheder, fuldmagt og samtykke), portaler og Digital Post. Myndigheden kan bygge på sikkerheden i disse komponenter (som beskrevet i fx referencearkitektur for brugerstyring) og skal i sin sikkerhedspolitik tage højde for, at sikkerheden i myndighedens egen løsning er afhængig af sikkerheden i den samlede kæde af komponenter og infrastruktur. I afsnittet om [krav til sikkerhed](/node/1100#krav-til-sikkerhed) beskrives dette.

Selvbetjeningsløsninger på internettet er udsatte for en række risici, og de skal derfor følge krav til cybersikkerhed både i løsningerne selv, men også i forhold til risici i brugernes udstyr og deres anvendelse heraf.

### Principper

#### Overblik over principper

Referencearkitekturen for selvbetjening fastlægger følgende principper for at styre frem mod en fælles forretnings- og it-arkitektur for det offentliges selvbetjeningsløsninger. Som overordnet ramme for disse principper for selvbetjening, anvendes de otte principper i Hvidbogen for arkitektur for digitalisering (dog ikke gengivet her).

Princip:

1. Brugerne møder i det enkelte selvbetjeningsforløb både forberedelse, kernen og afrunding, understøttet af digitale løsninger, der imødekommer brugernes behov.
2. Selvbetjeningsløsninger er forståelige, nemme og intuitive at anvende for brugerne.
3. Brugerne leverer kun information, som det offentlige ikke allerede har.
4. Brugerne oplever en sammenhængende service, også på tværs af myndigheder.
5. Brugerne skal altid kunne se, hvilken myndighed der er ansvarlig for at levere en tjeneste.
6. Myndigheder, der samarbejder om at kæde selvbetjeningsforløb sammen, aftaler opgave- og ansvarsfordeling inden for gældende regler.

#### Uddybende beskrivelse af principper

##### #1 Brugerne møder i det enkelte selvbetjeningsforløb både forberedelse, kernen og afrunding, understøttet af digitale løsninger, der imødekommer brugernes behov

Selvbetjeningsløsninger skal forberede brugeren på selvbetjeningsforløbet, gennemføre kernen brugervenligt og efterfølgende afrunde den med relevant information. Selvbetjeningsforløbet skal understøttes med digitale løsninger, der understøtter brugernes behov både i forhold til brugerapparater, brugssituationer og brugernes forudsætninger. 

Rationale

* For brugere er offentlige selvbetjeningsløsninger ofte den eneste  eller den letteste vej til en offentlig ydelse eller tjeneste eller til at udføre opgaver pålagt af det offentlige. Det er derfor en del af myndighedernes forpligtelse at gøre selvbetjeningsløsningerne brugervenlige og indrette dem efter brugernes behov og i balance med myndighedernes behov for oplysninger og tilkendegivelser.
* Selvbetjeningsløsninger skal indtænke analoge trin (fx hjælp til selvbetjeningsløsningen med telefonsupport, medbetjening).

Implikationer

* Myndighederne skal indrette selvbetjeningsløsninger med en forberedelse indeholdende vejledning og afklaring af brugerens behov, en forståelig og effektiv kerne med spørgsmål og svar samt information om det videre forløb i afrundingen.
* Selvbetjeningsforløb skal tilrettelægges med brug af digitale løsninger, der understøtter forskelligartede brugerbehov, herunder forskelligt brugerudstyr.

##### #2 Selvbetjeningsløsninger er forståelige, nemme og intuitive at anvende for brugerne

Selvbetjeningsløsninger tilrettelægges og opbygges, så de er forståelige, nemme og intuitive at anvende for brugerne. Der skal i ordvalg, information og design tages udgangspunkt i brugernes situation og behov.

Rationale

* For at brugere kan få dækket behov på en hurtig, brugervenlig og effektiv måde, skal selvbetjeningsløsninger være forståelige, nemme og intuitive at anvende for brugerne i de situationer, der fører til, at de skal bruge selvbetjeningsløsningen.

Implikationer

* Myndigheder og udviklere tilrettelægger selvbetjeningsløsningerne, så ord, informationer og designelementer er forståelige og funktionelt genkendelige for brugerne. Det betyder, at myndigheder og udviklere har viden om god praksis og gængse metoder for selvbetjeningsløsninger og indretter deres løsning herefter. 
* Myndigheder og udviklere balancerer hensynet til begreber og informationer, der er forståelige for brugere af selvbetjeningsløsningen, med hensynet til de begreber, der anvendes på fagområdet, samtidig med at de så vidt muligt også tager hensyn til brugernes forudsætninger og forståelsesramme.
* Brugergrænsefladen bør tilpasses målgruppen, eventuelt med mulighed for at vælge flere alternativer, hvor det er relevant.

##### #3 Brugerne leverer kun information, som det offentlige ikke allerede har

Brugerne skal i deres brug af selvbetjeningsløsninger kun aflevere information, som det offentlige ikke allerede har. 

Princippet skal og kan kun efterleves, såfremt den nødvendige information er tilgængelig for selvbetjeningsløsningen. Princippet bygger på målsætningerne om, at myndigheder skal anvende standarder for data og have snitflader til systemer. I de tilfælde, hvor nødvendig information ikke er tilgængelig, skal myndigheden rejse behovet i relevante samarbejds- og styringsorganer.

Rationale

* Brugere skal i stadig mindre omfang inddatere information og sjældnere opleve, at det offentlige beder om de samme oplysninger flere gange.
* Brugere undgår situationer, hvor de må opgive at gennemføre et selvbetjeningsforløb, fordi de ikke har adgang til den information, der efterspørges. Tilsvarende opnår myndighederne flere gennemførte selvbetjeningsforløb.
* For udviklings- og supportfunktioner betyder det, at de vil få mere tilfredse brugere og fx færre supporthenvendelser fra brugere, der ikke kan finde ud af at anvende selvbetjeningsløsningen, fordi de ikke kan finde den nødvendige information.
* Dette vil også bidrage til at sikre høj datakvalitet, da data, indsamlet af en myndighed, er underlagt krav til datakvalitet og skal være kvalitetssikrede.

Implikationer

* Brugere skal i den enkelte selvbetjeningsløsning (som udgangspunkt) kun inddatere information, som det offentlige ikke har i forvejen.
* Det indebærer, at det offentlige skal opbygge løsninger til sikkert og effektivt at lagre og dele inddateret information og anvende aftalte integrationsmønstre (hvilket kræver en langsigtet indsats). Den enkelte selvbetjeningsløsning skal efterleve princippet i det omfang, det er muligt at hente og aflevere data til fællesoffentligt brug . 
* Brugere skal have sikkerhed for, at den præsenterede information er korrekt, og der skal være klare regler for, hvad brugeren skal gøre, hvis informationen vurderes ikke at være korrekt. Selvbetjeningsløsningen skal da kunne håndtere at agere korrekt på en sådan påstand og have afklaret, om brugeren henvises til informationskilden, eller om informationen skal rettes i selvbetjeningsløsningen.
* Myndigheder og udviklere skal i tilrettelæggelsen af løsningen kortlægge, hvorfra de nødvendige informationer til selvbetjeningsforløbet og den tilhørende sagsbehandling kan indhentes og dernæst indhente den derfra. Denne kortlægning omfatter både juridiske , tekniske og andre relevante forhold. Den skal også omfatte eventuelle ændringer i indhentet information, hvis selvbetjeningsforløbet gennemføres over længere tid, fx ved afbrydelse og genoptagelse.
* Hvis der kræves samtykke til at indhente oplysninger, skal dette indhentes som del af selvbetjeningsløsningen.

##### #4 Brugerne oplever en sammenhængende service, også på tværs af myndigheder

Brugerne skal opleve en sammenhængende service, også når den går på tværs af flere myndigheder eller forvaltningsområder i en myndighed. Opgaveløsningen skal så vidt muligt tilrettelægges efter brugernes perspektiv uanset myndighedsskel .

Rationale

* Brugere opnår bedre service fra det offentlige, når selvbetjeningsløsninger løser sammenhængende opgaver, set fra brugernes synsvinkel.
* Brugere får løsninger, så de får bedre understøttelse og vejledning i deres livssituation, og i mindre omfang selv skal sørge for, at alle dele af en livssituation eller virksomhedssituation bliver håndteret (eller alternativt ikke bliver håndteret).
* Det offentlige løser den vejledningsforpligtelse, der fremgår af forvaltningslovens § 7.
* For udviklings- og supportfunktioner betyder det, at de vil få mere tilfredse brugere og fx færre supporthenvendelser fra brugere, der ikke kan finde ud af at løse en given opgave.

Implikationer

* Myndigheder og udviklere skal i tilrettelæggelse af selvbetjeningsløsningen understøtte sammenhængende brugerrejser, bl.a. ved at afklare hvilke selvbetjeningsforløb i myndigheden og i andre myndigheder der indgår i livs-/virksomhedssituationen. Det skal ske ud fra en vurdering af, hvor der indgår væsentlige forhold for brugerne, fx hvis der er lovgivningsmæssige krav, der fordrer en sammenhæng . 
* Hvis der indgår andre selvbetjeningsforløb i livs-/virksomhedssituationen, bør myndigheden bidrage til at sikre, at der skabes en sammenhængende service. Det kan ske i én løsning eller i flere løsninger, hvor der med relevante midler skabes sammenhæng for brugerne.
* Myndighederne skal tilrettelægge forløbene, således at forløbene så vidt muligt tager højde for, at brugerne kan have forskellige ønsker i forhold til, hvilke sammenhænge opgaverne skal løses i og i hvilken rækkefølge og tidsmæssig udstrækning.
* Hvis det skal være muligt for andre end brugeren selv at benytte selvbetjeningsløsningen, skal der være mulighed for, at en repræsentant kan anvende løsningen (med brug af fællesoffentlig fuldmagtsløsning).
* Når der tilrettelægges selvbetjeningskæder, skal de deltagende myndigheder i kæden i fællesskab aftale, hvordan brugerrejsen for hele kæden optimeres, således at overdragelsen mellem to selvbetjeningsforløb er så enkel som mulig for brugeren. Omfanget og karakteren af samarbejdet og governance afhænger af, hvordan sammenhængen planlægges realiseret. En relativt løst koblet sammenhæng kræver meget lidt governance, mens et samarbejde mellem flere myndigheder om sammenkædning af løsninger kræver omfattende governance.

##### #5 Brugerne skal altid kunne se, hvilken myndighed der er ansvarlig for at levere en tjeneste

Oplysninger om den ansvarlige myndighed skal præsenteres klart og gennemskueligt, særligt i selvbetjeningskæder der omfatter flere myndigheder, så det er synligt, hvilken myndighed der har ansvaret for en tjeneste, og den betjening af borger og virksomhed, som det omfatter.

Rationale

* Brugere skal til enhver tid kunne se, hvilken myndighed der er ansvarlig for en tjeneste, som brugeren anvender, for at vedkommende kan henvende sig med spørgsmål og klager.

Implikationer

* Myndigheder og udviklere skal i tilrettelæggelsen af løsningen sikre, at brugerne kan få information om den ansvarlige for et selvbetjeningsforløb eller dele heraf. Det indebærer, at myndigheden skal kende det lovmæssige ophæng (hvordan dette præsenteres for brugeren afgøres efter princip 3).
* Særligt for selvbetjeningsløsninger på portalerne er der behov for klar information om og support til at få hjælp til at løse opgaven, herunder hvor brugeren får support.
* Denne information skal tage hensyn til brugerens behov (fx hvor får jeg hjælp) og ikke myndighedens behov (præcisering af hvad myndigheden ikke gør).

##### #6 Myndigheder, der samarbejder om at kæde selvbetjeningsforløb sammen, aftaler opgave- og ansvarsfordeling inden for gældende regler

Når myndigheder samarbejder om at gøre deres selvbetjeningsforløb til en del af en sammenhængende brugerrejse, skal myndighederne samarbejde om dette og aftale opgave- og ansvarsfordeling.

Rationale

* Princippet ”Brugerne oplever en sammenhængende service, også på tværs af myndigheder” indebærer, at der skal være selvbetjeningskæder, der går på tværs af myndigheder. Der vil som følge heraf være behov for et samarbejde mellem myndigheder og/eller mellem myndigheder og myndigheder, der varetager infrastrukturkomponenter og portaler, og aftaler om opgave- og ansvarsfordeling mellem dem. 
* En sådan opgave- og ansvarsfordeling skal bidrage til, at brugerne oplever en sammenhængende service, både når selvbetjeningsløsningen fungerer optimalt, og når den ikke gør.

Implikationer

* Når to eller flere myndigheder har identificeret et behov for at samarbejde om en sammenhængende brugerrejse gennem en kæde af selvbetjeningsforløb, skal de som led i samarbejdet aftale samarbejdsformer, opgaveløsning og ansvarsfordeling både vedrørende udvikling, drift, support og andre relevante forhold. 
* Hvor flere myndigheder samarbejder om en sammenhængende brugerrejse gennem en kæde af selvbetjeningsforløb, skal der aftales brug af begreber og information.
* Myndighederne skal aftale ansvar for data, herunder eventuelt fælles dataansvar (jf. databeskyttelsesforordningen, artikel 26).
* Aftalen om opgave- og ansvarsfordeling kan omfatte, at en myndighed er ansvarlig for den samlede kæde af selvbetjeningsforløb inden for gældende regler om myndigheders ansvar.
* I nogle domæner har en portal opgaver i samarbejdet om en sammenhængende brugerrejse (fx virk.dk på virksomhedsområdet og borger.dk på borgerområdet).

## Del B Forretningsarkitektur

### Begrebsmodel

I dette afsnit beskrives en terminologi og begrebsmodel for selvbetjeningsforløb. Begrebsmodellen er på et generelt og overordnet logisk niveau. Det betyder, at den ikke er bundet til en bestemt type person, organisation, anvendelse eller implementering.  

![Figur 4.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%204.jpg)

Figur 4. Begrebsmodel for selvbetjeningsforløb

Referencearkitektur for selvbetjening definerer begreberne i figuren ovenfor til at være de termer, som anvendes fællesoffentligt i kommunikation og debat om selvbetjeningsforløb og sammenkædning af disse. Tabellen nedenfor definerer og beskriver disse termer, i alfabetisk rækkefølge.

|                         |                                                                                                      |
| ----------------------- | ---------------------------------------------------------------------------------------------------- |
| Modelnavn               | Digital selvbetjening                                                                                |
| Modelejer               | Digitaliseringsstyrelsen                                                                             |
| Versionsnummer          | 1.0.2                                                                                                |
| Seneste opdateringsdato | 01-08-2025                                                                                          |
| Modelstatus             | Stabil                                                                                               |
| Godkendelsesstatus      | Godkendt                                                                                             |
| Forretningsområde       | 06.38.10.10 Arkitektur for den digitale infrastruktur                                                |
| Juridisk kilde          | [https://www.retsinformation.dk/eli/lta/2015/1309](https://www.retsinformation.dk/eli/lta/2015/1309) |
| Kilde                   | Fællesoffentlig referencearkitektur for selvbetjening                                                |

| Term                     | Definition                                                                                                                                                                  | Note                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | Kilde                                 |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- |
| afrunding                | Del af selvbetjeningsforløb, som giver bruger informationer om konsekvenser og anviser det videre forløb.                                                                   | En afrunding består af en beskrivelse af den (nye) kontekst, som kernens forløb har bragt brugeren i, hvilke konsekvenser den ændrede kontekst har for brugeren og anvisning af et videre forløb, hvis dette er relevant.<br><br>Alternativ term: rekontekstualisering.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | Referencearkitektur for selvbetjening |
| betaling                 | At betale et beløb for en vare, en tjenesteydelse.                                                                                                                          | Nogle services eller produkter, der leveres gennem brugerrejse, er belagt med gebyrer eller pris, som skal betales.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Den Danske Ordbog Den Danske Ordbog   |
| brugerprofil             | En samling karakteristiske træk eller egenskaber ved en bruger af offentlige digitale løsninger.                                                                            | Det er muligt gennem analyser af data, genereret af en bruger, at karakterisere denne bruger af selvbetjeningsforløb: Sådanne karakteristika kan anvendes til at tilpasse brugerflade og brugerinteraktion, således at den pågældende brugerprofil nemmere kan udføre selvbetjeningsforløbet.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Referencearkitektur for selvbetjening |
| brugerrejse              | En brugers oplevelse af et selvbetjeningsforløb eller en selvbetjeningskæde.                                                                                                | Begrebet bruges, når synsvinklen er brugerens behov.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | Referencearkitektur for selvbetjening |
| brugervejledning         | Vejledning i, hvordan man bedst gennemfører brugerrejsen, herunder anvender selvbetjeningsløsningen.                                                                        | Selvbetjeningsforløbet støttes af vejledning til brugerne om gennemførelsen af forløbet. Det er materiale med råd, retningslinjer og instruktioner i at gennemføre selvbetjeningsforløbet.<br><br>Brugervejledninger kan være målrettet brugerprofiler.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | Referencearkitektur for selvbetjening |
| datavalidering           | Kontrol af, at data overholder krav.                                                                                                                                        | Når brugeren leverer informationer via sin enhed (apparat), sker der validering af leverede data med henblik på at opnå den bedst mulige datakvalitet.<br><br>De krav, der skal overholdes, er givet af det niveau af sikkerhed og af overholdelse af forretningsregler, som er aktuelt for det konkrete selvbetjeningsforløb.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Referencearkitektur for selvbetjening |
| digital selvbetjening    | Selvbetjening via internettet af en bruger, som anvender en digital brugerflade.                                                                                            | Denne referencearkitektur har fokus på interaktiv, internetbaseret kommunikation i modsætning til selvbetjening, fx det at finde varer i et supermarked.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Referencearkitektur for selvbetjening |
| forberedelse             | Del af selvbetjeningsforløb, der hjælper brugeren med at afklare forudsætningerne for at løse opgaven i kernen.                                                             | Forberedelsen består af sprogvalg, introduktion, interaktiv afklaring og kan indeholde et interaktivt brugerbidrag.<br><br>Forberedelsen giver informationer til brugeren og kan indsamle informationer. Disse informationer kan lagres i selvbetjeningskonteksten.<br><br>Dele af forberedelse kan ske i en portal, hvor selvbetjeningsforløbet beskrives, og noget af eller hele den interaktive afklaring foregår, hvorefter leder brugeren over til selvbetjeningsforløbets forberedelse eller kernen.                                                                                                                                                                                                                                                                                                                                                           | Referencearkitektur for selvbetjening |
| genoptagelse             | Fortsættelse af et afbrudt selvbetjeningsforløb.                                                                                                                            | Informationer, oplyst af brugeren i selvbetjeningsforløbet, lagres, så de er til stede, så længe brugeren ønsker det (og under iagttagelse af lovgivning, praksis m.m. ift. opbevaring af data). Dette gør det muligt at sætte selvbetjeningsforløbet på pause, forlade og genoptage det på et senere tidspunkt med alle informationer intakte.<br><br>Genoptagelse kan implementeres ved, at der eksisterer en kladde, som brugeren kan tage udgangspunkt i, hvis det ønskes, og givet, at data fortsat er aktuel.                                                                                                                                                                                                                                                                                                                                                  | Referencearkitektur for selvbetjening |
| interaktiv afklaring     | Afklaring, som opnås ved, at brugeren gennemgår en serie spørgsmål/svar.                                                                                                    | Disse giver brugeren en afklaring af, om vedkommende er på vej ind i det rette selvbetjenings­forløb, afstemmer forventninger om resultater af selvbetjenings­forløbet og forbereder brugeren på, hvad vedkommende eventuelt skal bidrage med.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Referencearkitektur for selvbetjening |
| interaktivt brugerbidrag | Brugerbidrag, hvor brugeren afgiver eller godkender informationer ved at interagere med en it-løsning.                                                                      | Det er gennem det interaktive brugerbidrag, at brugeren afgiver informationer og de handlinger, som opgaven kræver.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Referencearkitektur for selvbetjening |
| introduktion             | En indførende, forklarende fremstilling.                                                                                                                                    | En introduktion til et selvbetjeningsforløb er tekst, tegninger, billeder eller videoer, der leder brugeren frem til en interaktiv afklaring eller et interaktivt brugerbidrag.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | Den Danske Ordbog                     |
| kerne                    | Del af selvbetjeningsforløb, hvor brugeren gennemfører og løser selvbetjeningsforløbets opgave.                                                                             | En kerne består af interaktive brugerbidrag, hvorigennem brugeren afgiver de nødvendige informationer og accepterer eller godkender i selvbetjeningsforløbet. Kernen afsluttes med kvittering og/eller servicegodkendelse og/eller betaling.<br><br>Det er gennem kernen, at såvel bruger som myndighed skal opnå de resultater, informationer og/eller den viden, som blev afstemt i forberedelse. Kernen kræver, at brugeren er logget ind på det sikkerhedsniveau, som udførelsen af opgaven kræver.<br><br>Alternativ term: gennemførelse.                                                                                                                                                                                                                                                                                                                       | Referencearkitektur for selvbetjening |
| kontekstbestemt hjælp    | Hjælp i form af instruktioner til den aktivitet, brugeren er i gang med at udføre.                                                                                          | Selvbetjeningsforløbets brugerflade skal indeholde en kontekstbestemt hjælp, der relaterer sig til det konkrete trin i selvbetjenings­forløbet, som brugeren befinder sig på og hjælper brugeren igennem.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Referencearkitektur for selvbetjening |
| kvittering               | Dokumentation for de informationer og dokumenter, brugeren har leveret i forberedelse eller kernen.                                                                         | Når opgavens aktiviteter er gennemført, skal brugeren have en eller flere tilbagemeldinger på, hvordan forløbet er gået, og om resultaterne er modtaget og overtaget.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | Referencearkitektur for selvbetjening |
| overdragelse             | Del af selvbetjeningsforløb, som faciliterer en sammenkædning mellem to selvbetjeningsforløb, så dette sker forståeligt og operationelt for brugeren.                       | Overdragelse kan finde sted, når et selvbetjeningsforløb giver anledning til, at der skal løses flere opgaver gennem et eller flere selvbetjeningsforløb, således at forløbene kan kædes sammen i en selvbetjeningskæde.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Referencearkitektur for selvbetjening |
| overdragelsesaftale      | En organisatorisk specifikation og aftale om, hvordan et selvbetjeningsforløb tilknyttes et efterfølgende selvbetjeningsforløb.                                             | Overdragelsesaftalen indeholder de forretningsmæssige krav, til med hvilke kvaliteter en overdragelse skal finde sted, herunder krav til datasikkerhed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | Referencearkitektur for selvbetjening |
| overdragelses-kontekst   | Den delmængde af en selvbetjeningskontekst, som overdrages ved overdragelse.                                                                                                | Da overdragelse kan ske på tværs af myndigheds- og ressortgrænser, skal der tages stilling til, om kun dele af selvbetjeningskonteksten kan overdrages, og om der skal indhentes samtykke.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | Referencearkitektur for selvbetjening |
| sammenkædning            | En teknisk specifikation og funktion, der knytter et selvbetjeningsforløb til et efterfølgende selvbetjeningsforløb.                                                        | En sammenkædning specificerer tekniske kvalitetskrav til, hvordan to selvbetjeningsforløb kan knyttes sammen teknisk, således at der kan realiseres en hel eller delvis automatisk overdragelse og igangsætning af næste selvbetjeningsopgave.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Referencearkitektur for selvbetjening |
| selvbetjeningsforløb     | Sammenhængende række af aktiviteter, hvor borgere og virksomheder med en digital brugerflade udfører opgaver i relation til offentlig forvaltning eller virksomhed.         | Et selvbetjeningsforløb består af mindst tre dele: forberedelse, kernen og afrunding.<br><br>Efter en afrunding kan et selvbetjeningsforløb derudover bestå af en overdragelse til et andet selvbetjeningsforløb.<br><br>I selvbetjening udfører en bruger opgaver gennem et digitalt interface som fx at ansøge, indberette, indhente information om egne forhold i stedet for, som det var tilfældet tidligere, at løse opgaverne gennem udfyldelse af papirblanketter, indsendelse af breve, telefoniske henvendelser eller personligt fremmøde.<br><br>Hvor en brugerrejse indebærer gennemførelse af flere selvbetjeningsforløb, som skal kædes sammen, anvendes begrebet ”selvbetjeningskæde”.<br><br>Alternative termer: offentligt digitalt selvbetjeningsforløb, digitalt selvbetjeningsforløb.<br><br>Eksempel: Søge økonomisk friplads til daginstitution | Referencearkitektur for selvbetjening |
| selvbetjenings-kontekst  | Alle relevante informationer, som er til stede på et givent tidspunkt i et selvbetjeningsforløb.                                                                            | Selvbetjeningskonteksten lagres løbende, så selvbetjeningsforløbet kan genoptages, hvis det afbrydes.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | Referencearkitektur for selvbetjening |
| selvbetjeningskæde       | Et antal selvbetjeningsforløb, kædet sammen gennem overdragelser, der tilsammen giver en bruger mulighed for at løse opgaver i en given livssituation gennem selvbetjening. | Selvbetjeningskæder kan være sammensat naturligt, fordi kun en udførelse af flere opgaver samlet set løser de opgaver, en bruger har i en given livssituation. Selvbetjeningskæder kan også have en mere tilfældig sammenhæng, hvor resultatet af en opgave åbner nye muligheder for brugeren.<br><br>Selvbetjeningskæder vil kunne sammenkæde opgaver på tværs af ressortområder.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | Referencearkitektur for selvbetjening |
| selvbetjenings-løsning   | It-løsning, der implementerer et selvbetjeningsforløb eller en del heraf.                                                                                                   | Begrebet bruges, når der er fokus på den tekniske løsning.<br><br>De kan være fællesoffentlige, fx som ved bestilling af NemID, eller de kan være domænespecifikke, fx som på sundhed.dk.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Referencearkitektur for selvbetjening |
| servicegodkendelse       | Accept af, at de interaktive brugerbidrag er i overensstemmelse med brugerens ønsker og behov og dermed accept af de betingelser, hvorunder brugerbidraget er afgivet.      | Det kan være en aktivitet i kernen, at brugeren skal bekræfte<br><br>*   læst information<br>*   de oplysninger, der er indtaste<br>*   anden information og valg, som brugeren har afgivet.<br>*   informationer hentet fra andre registre<br>*   eller de betingelser (fx Tro og love, samtykker etc.), som afgivelsen af oplysningerne sker under,<br><br>En servicegodkendelse kan dokumenteres med forskellig styrke og stærkest gennem en digital signering.                                                                                                                                                                                                                                                                                                                                                                                                   | Referencearkitektur for selvbetjening |
| sprogvalg                | Valg af sprog, der læses, skrives eller tales på.                                                                                                                           | Her vælges det sprog, som selvbetjeningsforløbet vil blive formidlet i. Ønsker man at adressere brugerne ud fra deres profiler, kan der vælges mellem forskellige persona, som man har defineret.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | Referencearkitektur for selvbetjening |
| videre forløb            | Del af afrunding, som beskriver, hvad brugeren kan forvente og skal gøre i den videre behandling af sagen.                                                                  | Del af afrundingen, der i tekst, tegninger, billeder eller videoer beskriver for brugeren, hvad der sker som resultat af brugerens bidrag.<br><br>Her beskrives fx, hvem den ansvarlige myndighed er, hvad brugeren skal gøre, hvad myndigheden gør, og hvilke tidsforløb brugeren kan forvente.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | Referencearkitektur for selvbetjening |

### Organisatorisk perspektiv

#### Forretningskapabiliteter

I dette afsnit beskrives de forretningskapabiliteter og de væsentligste tilknyttede arkitekturbyggeblokke i et organisatorisk perspektiv, der skal være til stede for at kunne realisere de gevinster, der lægges op til med referencearkitekturen. 

En kapabilitet er evnen til at udføre aktiviteter og derigennem opfylde et mål. Referencearkitekturen begrænser sig til at definere de kapabiliteter, som forvalter referencearkitekturens begreber. Derudover er der beskrevet en række forretningsservices og funktioner, der realiseres af andre referencearkitekturer, og som selvbetjening benytter sig af. 

De forretningsbehov, der er beskrevet i Kapitel 6, og principperne beskrevet i Kapitel 8, peger entydigt frem mod, at selvbetjeningsforløb både skal kunne stå alene og i nogle tilfælde indgå i selvbetjeningskæder.

Et selvbetjeningsforløb indeholder potentielt mange former for informationer og interaktioner mellem brugeren og myndigheden i forhold til en opgave og er grundlaget for brugerens oplevelse af myndighedens tjenester eller produkter, relateret til den opgave. For at realisere selvbetjeningsforløb og selvbetjeningskæder skal myndigheden implementere kapabiliteter, der understøtter brugerens brugerrejser, således at brugernes oplevelse optimeres. 

Kapabiliteter kan være evner hos personer, teknologier eller en kombination af personer, der bruger teknologier. Når vi tilrettelægger selvbetjeningsforløb som gode brugerrejser, skal følgende fire kapabiliteter kunne anvendes af brugere og informationsteknologi:

* Forberedelse
* Kernen
* Afrunding
* Overdragelse

Forberedelse, kernen og afrunding leder frem til, at brugeren har leveret de oplysninger og handlinger, der gør, at en sagsbehandling kan gennemføres. Sagsbehandlingen er ikke en del af selvbetjeningsløsningen, men løses i eller af fagsystemer. Sagsbehandlingen kan være simpel, fx modtage og lagre de indberettede data og tilhørende metadata. Sagsbehandlingen kan være kompleks og kan indebære manuelle og automatiserede processer eller en kombination heraf. 

Figur 5 viser en oversigt over de opgaver, der skal løses i forbindelse med selvbetjeningsforløb, samt de aktører og roller, som anvender selvbetjeningsforløb. Øverst vises de fællesoffentlige styringsrammer og guides, som gælder for selvbetjeningsforløb. Til at realisere kapabiliteterne er angivet en række forretningsprocesser, forretningsservices, forretningsfunktioner eller forretningsobjekter, der som minimum skal overvejes i realiseringen af de fire kapabiliteter.  
   
 

![Figur 5.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%205.jpg)

Figur 5. Kapabiliteter og aktører i selvbetjeningsforløb og selvbetjeningskæder

En tilrettelæggelse af et selvbetjeningsforløb skal altid omfatte vurderinger af, hvilken grad af forberedelse og afrunding der skal knyttes til kernen. Hvad der er den rigtige vægtning, afhænger af den opgave, selvbetjeningen skal løse. Ligeledes vil mange selvbetjeningsforløb ikke indeholde overdragelse. I tilfælde hvor overdragelse er relevant, er der en række forskellige måder, det kan understøttes på, der afhænger af de selvbetjeningsforløb, der kædes sammen. Det afgørende kriterium vil altid være, hvilken tilrettelæggelse der giver brugeren den bedste oplevelse af selvbetjeningsforløbet (kombineret med realiserbarhed).  
Forberedelse skal sikre, at det er den rette opgave, brugeren går i gang med, og at de nødvendige oplysninger er klar. Den skal sikre, at brugeren forstår, hvad der skal gøres og hvorfor, og at brugeren har fået afklaret evt. spørgsmål. Forberedelsen kortlægger brugerens kontekst og forudsætninger for at løse opgaven. 

Forberedelsen kan indrettes, så den løser behovene hos brugere med forskellige forudsætninger; både brugere, der behøver meget hjælp, og brugere, der skal kunne nå hurtigt gennem selvbetjeningsforløbet eller springe over forberedelsen. 

Forberedelsen vil ofte fungere som en tragt, der leder frem til kernen. Forberedelsen kan tilrettelægges med en række spørgsmål og svar, der fører til en afklaring hos brugeren for at løse den aktuelle opgave. Denne type spørgsmål/svar er en interaktiv afklaring, der sikrer, at brugeren kan løse den opgave, der udfoldes i kernen, og som skal lede til at indfri brugerens behov. Disse spørgsmål vil typisk kunne formuleres af en erfaren sagsbehandler for det emne, opgaven vedrører. En sådan sagsbehandler har gennem sit virke oplevet, hvad der har været af tvivlsspørgsmål hos brugeren, og kan være behjælpelig med at formulere svar og reagere på typiske svar. Dette kombineres med omhyggeligt at gennemtænke, hvordan brugeren vil opleve og forstå den opgave, der venter i kernen. 

En forberedelse kan være meget kort, hvis der fx er tale om indberetninger, der gentages med jævne mellemrum. Trænede brugere skal da kunne gå direkte i gang med opgaven, mens nye brugere skal kunne få en grundig og tilstrækkelig indføring i at gennemføre selvbetjeningsforløbet.

En del af forberedelse er at finde frem til det selvbetjeningsforløb, man skal bruge. Dette kan ske gennem mange forskellige informationskanaler, der indeholder en introduktion til, hvad et givent selvbetjeningsforløb kan udrette for brugeren. En introduktion leder brugeren gennem tekst, tegninger, billeder eller videoer frem til en interaktiv afklaring eller en interaktiv instruktion.

Det er vigtigt at gennemtænke brugerperspektiver på denne introduktion ud fra det forventede klientel til anvendelse af selvbetjeningsforløbet, fx gennem brugerinddragelse. Er klientellet meget forskelligartet, skal det overvejes at udarbejde flere introduktioner og afklaringsforløb, målrettet hver sin brugergruppe. Det er centralt, at informationsmængden er overkommelig for brugeren, ellers vil introduktionen ikke blive læst, og den interaktive afklaring ikke blive gennemført.

Som et led i dette skal det kunne faciliteres, at man til en start vælger det sprog, som man ønsker, at selvbetjeningsforløbet skal foregå i. Selvbetjeningsforløbet skal i stigende grad kunne tilgås på andre sprog end dansk, hvorfor et sprogvalg i stigende grad er nødvendigt. Dette sprogvalg skal gælde i hele selvbetjeningsforløbet.

Det er muligt at karakterisere sine brugere, selv om disse endnu ikke har identificeret sig gennem et login. En karakteristik kan fx være grader af digital modenhed. Hvis myndigheden har adgang til at generere sådanne brugerprofiler, skal forberedelse kunne udnytte dette. Det kan være et led i forberedelse, at brugeren identificerer sig med en valgt digital identitet, på et valgt sikringsniveau. Er dette tilfældet, skal forberedelse udnytte de informationer, som myndigheden må og kan trække fra offentlige grunddata, fra fagsystemer, fra et sags- og ydelsesoverblik og fra offentlige klassifikationer.

Afklaringen i forberedelse kan indeholde, at brugeren afgiver oplysninger. Sker dette, skal disse oplysninger dels lagres i en selvbetjeningskontekst for at kunne anvendes senere i de efterfølgende kapabiliteter, dels skal informationerne datavalideres gennem anvendelse af god programmeringsskik herfor. En vigtig faktor for at undgå tilbageløb til brugeren, når oplysningerne er afgivet, er at validere, om oplysningerne og deres kombinationer giver forretningsmæssig mening i forhold til de forretningsregler, som gælder for den efterfølgende automatiske eller manuelle sagsbehandling.

##### Kernen

Det er i kernen, at selve selvbetjeningsforløbets opgave skal udføres. Set fra brugerens perspektiv er dette et eller flere kontaktpunkter, hvorigennem brugeren gennemlæser og accepterer eller godkender og afleverer informationer, som skal indberettes eller anvendes til at ansøge om ydelser, tilladelse og lign. fra det offentlige. Set fra myndigheden er disse kontaktpunkter, hvorigennem myndigheden indsamler informationer i form af data, der er nødvendige for at udføre den forvaltningsopgave, myndigheden skal løse.

I kernen er det centrale element for at tilrettelægge den rette serie af spørgsmål/svar, der fører brugeren vellykket gennem løsning af opgaven, hvilket her kaldes det interaktive brugerbidrag.  
Det interaktive brugerbidrag kræver, at brugeren har givet sig til kende med en valgt digital identitet på et valgt sikringsniveau gennem et login, idet myndigheden skal vide, hvem man servicerer, eller hvem der indberetter, godkender eller ansøger. Med MitId implementeret, er der mulighed for, at bruger og myndighed kan fastlægge det minimale identitetskendskab og det minimale sikringsniveau, som en given opgave kan løses med. Dette opfylder den fællesoffentlige digitaliseringsarkitekturs fokus på privacy (privatlivets fred).

Når der er foretaget et login, skal det interaktive brugerbidrag udnytte de informationer, som myndigheden må og kan trække fra offentlige grunddata, fra fagsystemer, fra et sags- og ydelsesoverblik og fra offentlige klassifikationer, samt hvad der måtte være gemt i en selvbetjeningskontekst, der er til rådighed fra forberedelse, eller i en overdragelseskontekst, modtaget fra et andet selvbetjeningsforløb i forberedelse. Det er et væsentligt bidrag til, at brugeren oplever en god brugerrejse, at det interaktive brugerbidrag udnytter alle allerede kendte data, der er til rådighed, både gennem forudfyldelse i brugerfladen og gennem at være til rådighed for en validering mod forretningsregler. 

Det er i den forbindelse meget vigtigt at oplyse brugeren om, hvor man kan hente data fra, og hvorfor det er hjælp til brugeren, således at brugeren forbliver tryg ved at blive præsenteret for disse data. Brugeren skal også have mulighed for at gøre indsigelse, hvis brugeren mener, at de præsenterede data ikke er korrekte. Kernen skal da kunne håndtere at agere korrekt på en sådan påstand.

De afgivne oplysninger placeres dels i selvbetjeningskonteksten, dels i relevante fagsystemer. Inden de lagres, skal de datavalideres gennem anvendelse af værktøjer hertil. En vigtig faktor for at undgå tilbageløb til brugeren, når oplysningerne er afgivet, er at validere, om oplysningerne og deres kombinationer giver forretningsmæssig mening i forhold til de forretningsregler, som gælder for den efterfølgende automatiske eller manuelle sagsbehandling.

Det er centralt, at den interaktive afklaring er overkommelig for brugeren, ellers vil brugeren gå i stå i løsningen af opgaven. Hvad der er overkommeligt, er meget brugerbestemt, og det kan være nødvendigt at have flere interaktive forløb for den samme opgave, tilpasset forskellige brugerprofiler, for at forbygge henvendelser ad andre kanaler end det digitale selvbetjeningsforløb.

Med udgangspunkt i den bruger, der har identificeret sig, de informationer og handlinger, som brugeren foretager, de informationer, som myndigheden har til rådighed, og de forretningsregler, der gælder for opgaven, kan det være muligt helt at automatisere det interaktive forløb i kernen. 

Det sker allerede for en række forvaltningsopgaver, og i takt med at den fællesoffentlige digitaliseringsstrategi med dens vægt på sikkerhed, sammenhæng og datadeling realiseres, bliver det muligt at automatisere flere og flere forvaltningsopgaver. 

Derfor skal det altid undersøges i kernen, i hvilken grad myndighedens deltagelse i det interaktive forløb kan automatiseres helt eller delvist. Enhver automatisering skal ske på baggrund af en forudgående afklaring af risici for at omgå den automatiske sagsbehandling fulgt af en imødegåelse heraf, såvel som at automatiseringen også skal være nyttig set fra brugernes perspektiv.

I nogle selvbetjeningsforløb skal brugeren betale for den ønskede ydelse eller evt. for et skyldigt beløb. I de tilfælde skal der være en service for betaling, der omfatter valg af betalingsform, indtastning af betalingsoplysninger, godkendelse heraf og overførsel af betalingsinformation til selvbetjeningsløsningen, så forløbet kan færdiggøres.

I selvbetjeningsforløb kan det være vigtigt, at brugeren godkender de informationer, der er afgivet, eller bekræfter, at man har foretaget de afgivne handlinger. Der skal derfor være adgang til en servicegodkendelse, der kan indeholde oversigt/opsummering af det indtastede/valgte og en knap med ”godkend”. I de tilfælde, hvor brugerens login ikke har tilstrækkeligt med identitetsinformationer eller et tilstrækkeligt sikringsniveau i forhold til en servicegodkendelse, skal der tilføres attributter, og/eller sikringsniveauet skal hæves. Endelig kan det være relevant at gennemføre en signering, hvis opgaven tilsiger dette høje krav til en valid servicegodkendelse.

Brugeren skal have mulighed for at danne en kopi af kernens resultat og enten gemme denne i læsbar form (Digital Post er en mulighed) eller kunne printe den. Som afslutning på kernen skal der altid gives en kvittering, der informerer om, at opgaven i kernen er afsluttet og med hvilket resultat. Der meddeles, hvilke informationer der er afgivet, og hvilke handlinger der er gennemført.

##### Afrunding

I afrunding skal brugeren orienteres om det videre forløb, givet den nye situation som gennemførelsen af kernen har bragt brugeren i, hvad brugeren evt. har af handlemuligheder samt tidsforløbet, før en afgørelse er truffet. Et videre forløb er en beskrivelse i tekst, tegninger, billeder eller videoer, der beskriver dette for brugeren.

Det er vigtigt for brugeren at kunne overskue og vide, om der vil være en straksafgørelse, eller der skal sagsbehandles. I begge situationer skal brugeren vide, hvem i myndigheden der er ansvarlig, og hvem man kan henvende sig til. Samtidig vil en afgørelse, straks eller senere, ændre brugerens situation – vedkommende modtager, fx en ydelse eller tilladelse eller afslag. 

Modtager brugeren ydelsen eller tilladelsen, giver det ofte vedkommende nye pligter og evt. nye muligheder (fx for andre services eller ydelser), som det er vigtigt, at brugeren forstår og har overblik over. Får brugeren afslag, kan brugeren – ud over muligheden for at klage – have alternative muligheder, som er vigtige at blive orienteret om på en måde, vedkommende kan forstå og handle på.

Endelig skal der i afrunding tages stilling til, hvad der skal ske med selvbetjeningskonteksten for dette selvbetjeningsforløb. Er der aftalt en sammenkædning med et andet selvbetjeningsforløb, går selvbetjeningskonteksten videre til behandling i overdragelse. Afsluttes selvbetjeningsforløbet, skal afrunding føre en kort dialog med brugeren, om brugeren vil lade myndigheden beholde hele eller dele af selvbetjeningsforløbet, fx til brug for at uddybe brugerens profil, med henblik på at fremtidige forløb bliver mere målrettet brugeren. Dette kan myndigheden have tilladelse til allerede, men det kan også kræve, at brugeren afgiver sit samtykke hertil.

##### Overdragelse

###### Forskellige overdragelsesformer

Når en situation for en bruger kræver, at der løses to eller flere opgaver, der har hver sit selvbetjeningsforløb, skal man gennem overdragelse sikre, at brugeren oplever brugerrejsen som smidig og sammenhængende. Overdragelse kan ske på flere måder. 

Sammenkædning af selvbetjeningsforløb er relevant, hvor der inden for en forholdsvis kort tidsperiode skal udføres flere opgaver i sammenhæng. Med en forholdsvis kort tidsperiode forstås et forløb, der varer få timer og højst få dage, hvilket har betydning for organiseringen af overdragelsen. Det indgår i overdragelsen, at myndighederne aftaler, hvor lang tid sammenhæng fastholdes, og dermed hvor længe overdragelseskonteksten lagres. Dette oplyses for brugeren.

Overdragelse kan i sin enkleste form ske ved, at brugeren fra afrundingen via et link føres videre til forberedelsen i det næste selvbetjeningsforløb. 

Overdragelse kan også ske ved, at to eller flere myndigheder går sammen om at koordinere et antal selvbetjeningsforløb, der ofte forekommer sammen, fx i forhold til en livssituation som det at starte en virksomhed. Dette kan myndighederne evt. lade en portal facilitere. En sådan koordinering kan i sin yderste konsekvens indebære en egentlig integration af flere forskellige myndigheders dele af brugerrejsen i ét samlet selvbetjeningsforløb.

Den enkleste form for overdragelse kan opnås, hvis selvbetjeningen deler brugerens status fællesoffentligt, og brugeren via portalerne (og andre steder, hvor data udstilles) selv bestemmer overdragelsens rækkefølge og tempo.

I en række situationer giver det ikke mening, at brugeren fortsætter umiddelbart med det næste selvbetjeningsforløb, da gennemførelsen af dette kan afhænge af myndighedens godkendelse af den ansøgning, indberetning eller lignende, som det netop afsluttede selvbetjeningsforløb førte til. Hvis afrundingen afdækker, at det efterfølgende forløb kan være relevant for brugeren (når og hvis myndighedens godkendelse opnås), kan brugeren tilbydes at modtage en notifikation  (advis), når det foregående forløb er afsluttet. Et eksempel herpå kunne være en bruger, der efter gennemførelse af et selvbetjeningsforløb, der ændrer husstands- eller indtægtsforhold, ønsker at søge en ydelse, der afhænger af disse forhold. 

##### Overdragelse af data

Myndighederne skal afklare behovet og mulighed for at overdrage information til næste led i en selvbetjeningskæde. Det sker med udgangspunkt i, at informationer om brugeren bør hentes fra grunddataregistre og derfor ikke er omfattet af overdragelsen.

Er overdragelse opnået med et link, vil der være begrænsede muligheder for at medsende data om det netop afsluttede forløb til at målrette det efterfølgende forløb.

Er der tale om en tættere koordination af selvbetjeningsforløbene kan oplysninger om de handlinger, der er foretaget – sammen med data fra den indledende afklaring – være en del af forberedelsen for det næste selvbetjeningsforløb. De data, myndigheden må og kan overdrage, lagres i overdragelseskonteksten . Når brugeren påbegynder næste skridt (aktiverer det næste selvbetjeningsforløb), medtages overdragelseskonteksten, således at forberedelse eller kernen i næste selvbetjeningsforløb kan tage eksplicit afsæt i det, brugeren har foretaget sig i det foregående selvbetjeningsforløb. Det bevirker blandt andet, at brugeren ikke bliver spurgt om det igen, og at selvbetjeningsforløbets flow fra starten er indrettet på de data, brugeren allerede har afgivet.

Myndighederne skal i samarbejdet om en selvbetjeningskæde afklare, hvilke informationer der skal overdrages. Som udgangspunkt forventes det at være procesinformation (fx muligheden for at se, at der ligger en indsendt, men endnu ikke behandlet, flytning), som er relevant for og valid nok til at sikre en sammenhængende brugeroplevelse. Det kan også være oplysning om afgivne informationer, som ikke er godkendt af myndigheden.

Det forventes ikke, at man lagrer informationer, som er tilgængelige i fagsystemer eller grunddata og lign., eftersom det ikke er givet, at brugeren starter det næste selvbetjeningsforløb med det samme. Dermed kan data, der er lagret i overdragelseskonteksten, være forældet, når man går i gang med det næste selvbetjeningsforløb. Man skal i stedet lagre links eller anden anvisning til, hvorfra data i fagsystemer eller grunddata og lign. kan hentes. 

Overdragelse kan ske såvel inden for samme ressortområde som mellem ressortområder. Gennem en sammenkædning specificeres kvalitetskrav til, hvordan to selvbetjeningsforløb kan knyttes sammen organisatorisk og teknisk med henblik på en automatisk overdragelse og igangsætning fra det første til det næste selvbetjeningsforløb.

Overdragelse af informationer kræver, at myndigheden har hjemmel til at videregive oplysningerne. Det kan myndigheden have ud fra lovgivning, men der er også situationer, hvor brugeren skal afgive et samtykke til, at hele eller dele af overdragelseskonteksten kan lagres og overgives til den næste afdeling, kontor, styrelse eller myndighed i rækken. Da der kan gå et tidsrum mellem, at et selvbetjeningsforløb afrundes og et nyt påbegyndes, skal brugeren have mulighed for at gøre indsigelse under forberedelse af næste selvbetjeningsforløb, hvis brugeren mener, at de præsenterede data ikke er korrekte. Forberedelse skal da kunne håndtere at agere korrekt på en sådan påstand.

##### Overdragelsesaftaler

Når der er tale om overdragelse mellem ressortområder, skal der udarbejdes en overdragelsesaftale , der blandt andet kan indeholde:

* En veldefineret angivelse af det punkt, hvor forvaltningsansvaret skifter fra det ene ansvarsområde til det næste.
* En fastlæggelse af, hvilke informationer der kan overdrages mellem ressortområderne.
* En fastlæggelse af, hvor lang tid en overdragelseskontekst lagres, og dermed hvor længe en selvbetjeningskæde opretholdes.
* De organisatoriske enheder og disses roller, der formidler skiftet i forvaltningsansvar.
* En databehandleraftale, der overdrager det at udføre selve den praktiske behandling af personoplysninger på den dataansvarliges vegne.

Når der er tale om overdragelse både inden for ressortområder og mellem ressortområder, skal der udarbejdes og aftales kvalitetsniveauer for datatransport og datas validitet. Dette handler om forretningsmæssigt at fastlægge kvalitetsniveauer for:

* Karakteristik af de informationer, der overdrages: Den begrebsmodel, der definerer betydningen af de data, der repræsenterer informationen, datas format og volumen, eventuelle metadata tilknyttet.
* Karakteristik af datakilden: validitet, aktualitet, følsomhed, gyldighed og lokation.
* Karakteristik af datatransporten: kommunikationsprotokol, initiativtager til overførslen, løs eller tæt sammenknytning, svartid, overførselstid (latency), frekvens, kapacitet, tilgængelighed, fortrolighed, pålidelighed og integritet, fejlhåndtering og monitering (logning).

Det er nødvendigt, at myndighederne fastlægger disse niveauer, idet valget af niveauer er en afvejning af de risici, der følger med valget af et niveau, og de omkostninger, som realiseringen af dette niveau medfører.

##### Forretningselementer, der anvendes i alle kapabiliteter

###### Selvbetjeningskontekst

En selvbetjeningskontekst består af alle relevante informationer, som er til stede på et givent tidspunkt i et selvbetjeningsforløb. Dette kan omfatte:

* Informationer, som brugeren har afgivet.
* Informationer, selvbetjeningsforløbet har hentet fra grunddata og fagsystemer eller fra overblik over sager og ydelser.
* Informationer fra en brugerprofil.
* Informationer om, hvordan selvbetjeningsforløbet er blevet gennemført. 
* Resultaterne af selvbetjeningsforløbet.

I de selvbetjeningsforløb, der realiseres med flere selvbetjeningsløsninger, fx i en portal og i en kerne, vil der være behov for, at selvbetjeningsløsningerne deler selvbetjeningskonteksten. Der kan også være behov for at indgå aftaler, svarende til dem der er beskrevet ovenfor under overdragelse.

Når selvbetjeningsforløbet er afsluttet, lagres (persisteres) de informationer, der er nødvendige for sagsbehandling og logning. Myndigheden skal afklare, om den har hjemmel til, at informationer kan anvendes til andre formål hos myndigheden, fx opdatering af brugerprofiler. Hvis ikke skal der indhentes samtykke.

![Figur 6.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%206.jpg)

Figur 6. Funktionaliteten af selvbetjeningskonteksten

###### Overdragelseskontekst

En overdragelseskontekst er den del af selvbetjeningskonteksten, som har relevans for et givent efterfølgende selvbetjeningsforløb, og som ikke kræver efterfølgende myndighedsgodkendelse eller verificering, før det kan anvendes i det efterfølgende forløb. Hvis overdragelsen sker på tværs af forvaltnings-/myndighedsgrænser, kræver det hjemmel eller et samtykke fra brugeren.

![Figur 7.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%207.jpg)

Figur 7. Funktionaliteten ”overdragelseskontekst”

###### Genoptagelse

Genoptagelse består i, at alle informationer, hentet frem eller afgivet, lagres i hele selvbetjeningsforløbet, således at det er muligt at sætte opgaveløsningen på pause, forlade selvbetjeningsforløbet og genoptage den på et senere tidspunkt med alle informationer intakte. Funktionen genoptagelse anvender en selvbetjeningskontekst som lager, og er der produceret dokumenter eller brugt andre medier, skal der også være adgang til at genoptage disse. Muligheden for genoptagelse skal have en tidsbegrænsning, og brugeren skal informeres om dette.

Genoptagelse kan aktiveres gennem en notifikation (advis), som brugeren modtager fra selvbetjeningsforløbet. Genoptagelse udfylder også den funktion, som giver adgang til en kladde, således at aktiviteterne i selvbetjeningsforløbet først betragtes som leveret, når brugeren specifikt giver besked om dette.

###### Vejledning

Vejledning kan bestå af en række forskellige elementer:

* En introduktion til brugeren om, at selvbetjeningsforløbet eksisterer, og at brugeren kan betjene sig selv uafhængig af tid og sted.
* En vejledning til, hvad der er nødvendigt at medbringe af oplysninger og adgangsbilletter for at gennemføre og besvare spørgsmål undervejs i selvbetjeningsforløbet.
* En vejledning til, hvilke apparater med hvilke brugerflader der kan anvendes til at tilgå selvbetjeningsforløbet.
* En henvisning til de love, betænkninger og regler, som er grundlaget for selvbetjeningsforløbet.
* En guide til, hvordan selvbetjeningsforløbet forløber.
* Adgang til support via chat, telefon og lign.

###### Hjælp

Hjælpen kan bestå af en række forskellige elementer, der alle tager udgangspunkt i konkrete situationer i selvbetjeningsforløbet og kan fortælle eller vise, hvordan dette trin i forløbet skal løses:

* Ledetekster, click up-tekster, mouse over-hjælp. 
* En assistent, guide eller wizard, der hjælper brugeren gennem løsningen.
* Link, hvorfra der kan hentes kontekstafhængig hjælp.
* Hjælpesider i en digital manual, som der kan søges i.
* Adgang til support via chat, telefon og lign.

##### Brugere af selvbetjeningsforløb

###### Aktører

Selvbetjeningsforløbenes aktører er borgere, udlændinge, virksomheder, ting eller systemer. Borgere er danske statsborgere, bosiddende i Danmark eller i udlandet, og som har et CPR-nummer. Udlændinge er udenlandske statsborgere, bosiddende i Danmark eller i udlandet.

Borgere eller udlændinge kan – ud over at være direkte aktører – optræde i rollen som bisidder. En bisidder er en af borgeren eller udlændingen valgt fortrolig, som assisterer en borger eller en udlænding i at gennemføre brugerrejsen.

Virksomheder som aktør optræder gennem følgende roller i virksomheden: ejer, medarbejder eller supporter. Dertil kan virksomheder optræde som rådgiver. Rådgiveren kan enten repræsentere virksomheden eller vejlede virksomheden. En medarbejder i en offentlig virksomhed, der leverer selvbetjeningsløsninger, kan optræde som rådgiver (medbetjener) eller supporter over for brugere af deres selvbetjeningsløsninger. 

Systemer kan afsende notifikationer (Digital post/SMS), der kan indgå i eller igangsætte et selvbetjeningsforløb. Et fagsystem kan fx igangsætte et selvbetjeningsforløb, evt. efter at forudsætningerne herfor er opfyldte. En implementering af et selvbetjeningsforløb kan fx indeholde afsendelse af en besked om, at man skal huske at afslutte sit selvbetjeningsforløb inden for en given frist. Eller at man på et givent tidspunkt skal fortsætte med det næste selvbetjeningsforløb i kæden, fordi de igangsatte aktiviteter i sagens behandling er afsluttet med et resultat, der betyder, at man kan gå videre.

Ting, kan også tilsvarende afsende notifikationer (advis). Med ting menes sensorer og apparater, fx i sundhedssektoren, landbruget og lign. Man kan eksempelvis forestille sig en sensor hos en hjemmeliggende patient, der igangsætter, at patienten gennem selvbetjening skal forklare omstændigheder og konteksten for et givent måleresultat. 

Alle aktører, der indgår i et selvbetjeningsforløb, hvor det er nødvendigt at kende deres identitet på et vist niveau af attributter og være autentificeret på et vist sikringsniveau, skal gennemføre et login. Dette login skal følge retningslinjerne i referencearkitektur for brugerstyring og anvende de fællesoffentlige forretningsservices hertil, således som det er beskrevet i [afsnittet om sikkerhed](/node/1100#sikkerhed).

###### Servicelevering af selvbetjeningsforløb

Selvbetjeningsforløb leveres gennem et antal forskellige digitale kommunikationskanaler og kommunikationsredskaber, som vælges af den myndighed, der har ansvaret for selvbetjeningen, medmindre der er aftalt andet. Brugeren skal gennem serviceleveringen præsenteres for et link, der igangsætter forberedelse af et selvbetjeningsforløb. 

Myndigheder kan - og skal - i mange tilfælde samarbejde med portaler og lade dele af et selvbetjeningsforløb afvikles der. Myndigheder kan også afsende en hændelse fra et fagsystem eller en ting gennem en snitflade og ad denne vej igangsætte et selvbetjeningsforløb.

##### Forretningselementer, der er defineret og beskrevet i andre referencearkitekturer

Denne referencearkitektur benytter sig af forretningsservices, forretningsfunktioner eller forretningsobjekter, som er defineret og beskrevet i andre referencearkitekturer. I følgende tabel gives en kort beskrivelse af disse forretningselementer, idet der i Bilag C henvises til de relevante dokumenter for disse referencearkitekturer.

| Tjeneste                       | Beskrivelse                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Adgang til grunddata           | Muligheden for at trække på allerede kendte grunddata, som er personer, virk-somheder, fast ejendom, adresser, veje og områder, vand og klima og geografi. Adgang kan gives, når der er foretaget et login.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Overblik over sager og ydelser | Dette overblik leverer et ønsket uddrag af sager eller ydelser vedrørende en aktuel bruger, når disse er relevante for det aktuelle selvbetjeningsforløb. Over-blik kan leveres, når der er foretaget et login.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Fagsystem Adgang               | Et selvbetjeningsforløb vil ofte levere data til et fagsystem. Fagsystemet kan til selvbetjeningsforløbet levere data, som det allerede kender, samt information om regler, der kan anvendes i datavalidering.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Adgang til klassifikationer    | Et selvbetjeningsforløb skal kunne trække på nyttige klassifikationer som fx KLE, FORM m.fl.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Notifikation (Advis)           | En selvbetjeningsløsning har brug for at kunne afsende besked om hændelser til brugerne og til andre myndigheder som led i overdragelse. Dette er denne tjene-stes opgave.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Login                          | På et tidspunkt under forberedelse og inden kernen skal brugeren foretage et login på et identitetsniveau og et sikringsniveau, der er bestemt af myndigheden. Et login kan formidles via adgangsbilletter, udstedt af andre myndigheder, såle-des at login foregår automatisk, fx gennem fællesoffentligt login.<br><br>Afhængig af, hvilke informationer selvbetjeningsforløbet behandler, kan det være nødvendigt under forløbet at hæve sikringsniveauet eller identitetsniveauet gen-nem fornyet login.<br><br>Login skal følge retningslinjerne i referencearkitektur for brugerstyring og anvende de fællesoffentlige forretningsservices hertil, således som det er beskrevet i [afsnittet om sikkerhed](/node/1100#sikkerhed) og [afsnittet om krav til sikkerhed](/node/1100#krav-til-sikkerhed). |
| Samtykke                       | Brugere af selvbetjeningsløsninger skal kunne afgive samtykke om:<br><br>*   At de informationer, brugeren har afgivet til myndigheden, kan videre-gives til andre myndigheder.<br>*   At myndigheden kan indhente informationer fra andre myndigheder.<br>*   At myndigheden i det hele taget må behandle data, selv om myndighe-den ikke har hjemmel til det.                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Fuldmagt                       | Brugere af selvbetjeningsforløb kan afgive fuldmagt til bisiddere eller rådgivere om, at de pågældende aktører kan læse og handle på en brugers vegne. Selvbe-tjeningsløsningens adgangskontrol skal kunne håndtere at kontrollere, om en fuldmagt er afgivet.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Signering                      | Brugere af selvbetjeningsforløb kan blive bedt om at bekræfte oplysninger og valg med en digital underskrift. Dette leveres af en fællesoffentlig signerings-komponent.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

#### Processer

Processer for selvbetjening kan have mange forskellige forløb og omfang. Det kan spænde fra at læse årsopgørelsen fra SKAT og ikke gøre noget, over et enkelt kort forløb til at løse alle opgaver i forbindelse med oprettelse af ny virksomhed – i bedste fald en kæde af sammensatte selvbetjeningsforløb.

I det følgende beskrives et enkelt selvbetjeningsforløb som nedenstående (uddrag af figur i [afsnittet om beskrivelse af emnet selvbetjening](https://fda-preprod.digst.govcloud.dk/node/1100#beskrivelse-af-emnet-selvbetjening)).

![Figur 8.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%208.jpg)

Figur 8. Enkelt forløb

Som gennemgående eksempel er valgt ansøgning om boligstøtte. Her beskrives processerne opdelt på:

•    Forberedelse, kernen, afrunding og overdragelse.

I praksis er der tale om en sammenhængende proces, der er tilrettelagt, så den opleves som én brugerrejse. I eksemplet er overdragelse konstrueret - det er ikke en del af det eksisterende selvbetjeningsforløb for boligstøtte. 

![Figur 9.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%209.jpg)

Figur 9. Proces for forberedelse

Selvbetjeningsforløbet kan startes ved at gå på borger.dk eller på kommunens hjemmeside for at orientere sig om, hvordan man søger boligstøtte. Her ledes man frem til selvbetjeningsforløbet, og når man klikker på linket, beder selvbetjeningsforløbet om et login via det fællesoffentlige eID , der identificerer ansøgeren gennem et to-faktor sikret certifikat. Herefter ledes brugeren gennem en interaktiv afklaring i tre trin, styret af selvbetjeningsløsningen. Der er undervejs i selvbetjeningsløsningen mulighed for at fremkalde hjælp eller vejledning. 

Hvor meget af forberedelse, der placeres på en portal, og hvor meget der ligger i selvbetjeningsløsningen er altid et konkret valg. I den udstrækning portalen kender en brugers kontekst, kan portalen tilpasse indholdet på baggrund af, hvad den ved om brugeren. Hvis borger.dk fx ved, at brugeren modtager boligstøtte, er folkepensionist og bor i Varde, så kan indholdet tilpasses hertil og dermed foretage en del af den interaktive afklaring.

Der vil være mange andre selvbetjeningsforløb, hvor forberedelsen er ganske kort eller helt kan springes over, fordi der er tale om et selvbetjeningsforløb, der gentages meget ofte og af de sammen medarbejdere hos virksomheder, som bliver trænet i at bruge selvbetjeningsløsningen. 

![Figur 10.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%2010.jpg)

Figur 10. Forberedelse - trin 1 og 2

I det tredje trin præsenteres brugeren for sin nuværende adresse, hentet fra grunddata, og brugeren oplyses om, hvor adressen kommer fra. Brugeren kan ændre denne adresse, hvis ikke det er der, der skal søges boligstøtte til. Adresseangivelsen bliver løbende valideret, efterhånden som den angives op imod et vejregister, således at der ikke kan søges boligstøtte til en fiktiv adresse.

![Figur 11.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%2011.jpg)

Figur 11. Forberedelse - trin 3

I hele selvbetjeningsforløbet er der hele tiden mulighed for at kontakte Udbetaling Danmark. Brugeren ledes til en side med oplysning om, at der sidder hjælpere parat i de fleste dag- og aftentimer. De oplysninger, man har afgivet i forberedelsen og senere i kernen, er gemt i en selvbetjeningskontekst, således de er til rådighed, hvis man ønsker at holde en pause i selvbetjeningsforløbet. Udbetaling Danmark oplyser gennem selvbetjeningsløsningen, at oplysningerne gemmes i tre måneder, og at ansøgningsforløbet ikke går i gang, før brugeren har indsendt ansøgningen. 

Når man er igennem afklaringen, er det sikret, at man starter korrekt på selvbetjeningsforløbets kerne.       
 

![Figur 12.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%2012.jpg)

Figur 12. Kernen i selvbetjeningsforløbet

I kernen præsenteres man for at skulle afgive alle de oplysninger, som skal bruges til at behandle ansøgningen.

![Figur 13.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%2013.jpg)

Figur 13. Trin i kernen og et eksempel

Brugeren hjælpes igennem hvert trin, og selvbetjeningsløsningen kender forretningsreglerne for at søge boligstøtte. Hvis brugeren fx angiver, at boligen ikke er en fast adresse, får man med det samme at vide, at man ikke kan få boligstøtte, og ansøgningsforløbet skal afsluttes, medmindre adressen tilrettes. 

Selvbetjeningsløsningen kan hente og opdatere grunddata om oplysninger på andre brugeres adresser og med eIndkomst for at hente indkomstoplysninger. Den validerer indtastningerne. Der er konstant kontekstnær hjælp, og man kan hele tiden få præsenteret de indtastede oplysninger i et resultatbillede. Herfra kan man gå frem og tilbage mellem de fem trin, som man nu har oplysninger til, og man kan uploade de dokumenter, en ansøgning kræver, man skal afgive som dokumentation.

![Figur 14.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%2014.jpg)

Figur 14. Vis resultat i kernen

Hele vejen gennem forløbet bliver oplysningerne valideret - også op imod forretningsregler. Når man fx kommer til tilføjelser og har leveret indkomstoplysninger, og disse medfører, at man ikke kan få boligstøtte, så meddeler selvbetjeningsløsningen, at man ikke kan opnå boligstøtte og derfor ikke skal indsende en ansøgning.

Til sidst kan brugeren inspicere resultatet af indtastningerne og gennem en markering angive, at oplysningerne er korrekte, og at brugeren afgiver samtykke til at indhente og videregive de oplysninger, der er nødvendige for at gennemføre ansøgningen. Med dette samtykke er man sømløst startet på selvbetjeningsforløbets afrunding.   
 

![Figur 15.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%2015.jpg)

Figur 15. afrunding og overdragelse

Når ansøgningen er sendt, kan brugeren opleve at modtage en straksafgørelse, hvis dette kan finde sted på grundlag af afgivne oplysninger og forretningsreglerne for at opnå boligstøtte. Mangler der at blive uploadet dokumenter, så oplyses det, at de skal være afgivet inden 14 dage, hvis ansøgningen skal vedblive at være valid. Kan der ikke afgives en straksafgørelse, så oplyses brugeren om det videre forløb i sagsbehandlingen, hvem brugeren kan kontakte, og hvornår en afgørelse kan forventes.

Hvis der af de oplysninger, som er afgivet i selvbetjeningsforløbet, kan udredes, at denne borger har mulighed for at søge hel eller delvis friplads til sine børn i institution, kunne der ske en overdragelse. Der skal ske indhentning af et fornyet samtykke, eftersom oplysningerne nu skal overdrages til en anden myndighed, og der i dette tilfælde ikke er hjemmel til blot at overføre oplysningerne. Derefter igangsætter overdragelsen en sammenkædning, der bygger på den overdragelsesaftale, der fx eksisterer mellem Udbetaling Danmark og kommunerne om at sammenkæde boligstøtteansøgningen med en fripladsansøgning. Fordelen er, at disse oplysninger nu kan indgå i forberedelsen af at søge friplads digitalt. Men som angivet i starten af afsnittet, er denne overdragelse et konstrueret eksempel blot med henblik på at illustrere overdragelse.

##### Andre selvbetjeningsforløb

I tilrettelæggelse af selvbetjeningsforløb skal der tages højde for, at der er mange forskellige selvbetjeningsforløb, og at der kan forventes flere og nye varianter.

For mange virksomheder er der ikke tale om et enkeltstående selvbetjeningsforløb, men en løbende indberetning til forskellige myndigheder. Det kan gennemføres ved, at der i forberedelse eller kernen er mulighed for at genbruge tidligere indberetninger, evt. med ændringer. Det skal også være muligt for trænede brugere at springe en forberedelse over og gå direkte til kernen. Selvbetjeningsløsningen skal tilpasses de typiske målgrupper. 

En meget anvendt mulighed for virksomheder er, at selvbetjening kombineres med maskinel indberetning. Derfor skal kernen kunne tilbyde en snitflade, der tillader en maskinel indberetning og en initiering fra det digitale værktøj, virksomhedens medarbejder anvender. Det kan være, at der er behov for at tilknytte funktionalitet i kernen, hvis der fx kræves servicegodkendelse eller kontrol af maskinelt indberettede oplysninger. Så skal disse muligheder bygges ind i snitfladen.

#### Portaler

Selvbetjeningsløsninger kan tilgås fra bl.a. myndighedens hjemmesider og fra fællesoffentlige portaler som borger.dk og virk.dk, hvor der via de fællesoffentlige aftaler også skal være adgang til myndighedernes selvbetjeningsløsninger.

Referencearkitekturen har som mål at styrke brugerens oplevelse af en sammenhængende offentlig service gennem fællesoffentlige kommunikationskanaler, så brugeren ikke på forhånd skal vide, hvilke myndigheder (med skiftende navne og ressortområder) der har ansvaret for en given opgave, før de kan komme i gang med at løse den. 

I tilrettelæggelsen af selvbetjeningsløsninger skal der tages højde for, om løsningen alene skal præsenteres i en portal eller både i en portal og på myndighedens hjemmeside m.m. Krav om en brugervenlig forberedelse og afrunding skal efterkommes i alle tilfælde, og i tilrettelæggelsen skal der tages højde for at sikre dette. Sammenhængen i selvbetjeningsforløb kan sikres af en portal, hvor selvbetjeningen foregår i brugerens optik, selv om løsningerne teknisk set er placeret hos myndighederne.

Der er forskellige aftalesæt og forpligtelser i forbindelse med de tre portaler, som myndighederne skal tage højde for i tilrettelæggelsen af selvbetjeningsløsninger.

## Del C Teknisk arkitektur

### Indledning

Fokus i dette afsnit er på at beskrive, hvilke tekniske komponenter der skal indgå i overvejelserne, når der skal udvikles selvbetjeningsløsninger efter denne referencearkitektur. Det gælder både de komponenter, der skal anvendes og/eller udvikles i den enkelte myndighed, og fællesoffentlige komponenter.

Selvbetjeningsløsninger kan realiseres med teknologiske muligheder, der omfatter både klassiske webløsninger, målrettede platforme, mobile apps og microservices. Området er præget af en hurtig og omfattende udvikling internationalt, og det har stor betydning for, hvordan forretningskapabiliteter realiseres i tekniske komponenter. Der eksisterer i markedet mange forskellige formularplatforme og udviklingsrammeværk, som alle i større eller mindre grad indeholder de nævnte applikationskomponenter, som denne referencearkitektur udpeger. ”Interaktive brugerbidrag” kan fx realiseres som enkeltstående formularapplikationer, som komponenter i CMS (Content Management Systems) og i processtyringsplatforme.

Rammearkitekturens anvisninger vedrørende applikationskomponenter og fællesoffentlige infrastrukturkomponenter beskriver den funktionalitet, som de forskellige dele bør have, med henblik på:

* At implementere selvbetjeningsforløb med velfungerende interaktive elementer til spørgsmål/svar og stor brug af allerede kendte data, som det offentlige har adgang til og har ret til at anvende i det konkrete selvbetjeningsforløb.
* At sikre lige stor vægt i tilrettelæggelsesfasen på forberedelse, kernen og afrunding samt overdragelse, når dette element indgår. Under tilrettelæggelsen afgøres, hvilken vægtning af kapabiliteterne der er den rette i den konkrete selvbetjeningsløsning. 

Komponentbeskrivelserne i Del C af vil derfor være abstrakte i den forstand, at komponenterne beskriver, hvad en løsningskomponent skal kunne gøre, og ikke hvordan komponenterne kan realiseres. I stedet skitserer [afsnittet om realiseringsmodeller](/node/1100#realiseringsmodeller) forskellige realiseringsmuligheder for komponenterne. Disse abstrakte beskrivelser er referencearkitekturens anvisninger til, hvad der bør indgå i realisering af selvbetjeningsløsninger. 

I de følgende afsnit vil først applikationskomponenter til den enkelte selvbetjeningsløsning blive gennemgået, og hvilke overvejelser myndighederne skal gennemløbe i forbindelse med valg af teknologier. Derefter præsenteres forskellige realiseringsmuligheder og slutteligt de fælles offentlige komponenter.

### Applikation

#### Komponenter

Figur 16. Mulige komponenter i selvbetjeningsforløb viser mulige komponenter til realisering af selvbetjeningsløsninger. Hvor mange og hvilke af dem man vil anvende, vil afhænge af det aktuelle selvbetjeningsforløb, som man har tilrettelagt. Det er vigtigt at huske, at forberedelse, kernen og afrunding leder frem til, at brugeren leverer de oplysninger og handlinger, der gør, at en sagsbehandling kan gennemføres. Sagsbehandlingen er ikke en del af selvbetjeningsløsningen, men løses i og af fagsystemer. 

Der er i beskrivelsen af komponenter i dette afsnit lagt vægt på at beskrive disse på en måde, så det ikke medfører krav om konkrete teknologier eller produkter. I [afsnittet om realiseringsmodeller](/node/1100#realiseringsmodeller) er der beskrevet mulige realiseringsmodeller for nogle af komponenterne.  
 

![Figur 16.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%2016.jpg)

Figur 16. Mulige komponenter i selvbetjeningsforløb

##### Brugerflader på brugerapparater

Selvbetjeningsforløb foregår gennem de enheder (apparater, devices), som brugerne er vant til at bruge. Dette betyder, at selvbetjeningsløsningens brugerflader skal konstrueres, således der kan anvendes både almindelig computerskærm, tablet, smartphones og specialapparater alt afhængig af de konkrete brugere af selvbetjeningsløsningen.

Derfor anbefales det, at brugerfladen implementeres med en løs kobling mellem brugerfladepræsentationen og de services og den funktionalitet, som er en del af selvbetjeningsforløbet. Dels for at gøre det nemt at skifte brugerflade, inklusiv at kunne bygge brugerfladen ind i et medarbejderværktøj eller i en portal, dels for at gøre det nemt at skifte apparat. Derfor bør alle services og den funktionalitet, som en brugerflade giver adgang til, også udstilles gennem et API (Application Programming Interface), valgt blandt de fællesoffentlige standarder herfor. Det skal dog først undersøges, om der er virksomheder (offentlige, private eller foreninger), der vil anvende dette API, da omkostningerne ved at udstille et API skal modsvares af et behov.

Konstruktionen af brugerflader skal gives høj opmærksomhed for at sikre et enkelt og intuitivt forløb og skal om nødvendigt tilpasses forskellige brugerprofiler. En designguide for brugeroplevelser vil kunne vejlede i konstruktion af brugerflader og brugeroplevelser (User Experience, UX). 

Konstruktionen af brugerflader skal tage højde for, at funktionshandikappede brugere kan anvende de digitale brugerflader, jf. Digitaliseringsstyrelsens retningslinjer for anvendelse af WCAG-standarden.

##### Indholdsstyring

Selvbetjeningsløsningen præsenterer tekst, lyd, tegninger, billeder, videos relevante for det konkrete selvbetjeningsforløb. Redigering, layout og navigation heraf samt kald af services og funktionalitet er det, komponenten indholdsstyring tager sig af. 

Til dette anvendes de relevante webteknologier, der også kan læses og tolkes af brugernes apparater. Derfor skal man bedømme, hvilke browsere eller operativsystemversioner brugerne har adgang til. Til brugerflader, der skal afvikles som mobile apps, skal man overveje, om der skal bruges native kodning af apps eller webteknologier til alle apparattyper. Det betyder, at applikationen kan have svagheder på nogle apparater, når det kommer til native kodning af apps, men vil være billigere og vil skabe sammenhængende løsninger på tværs af myndigheder.

Brugen af mobile apps kombineret med følsomme informationer kræver en høj beskyttelse af, hvad der befinder sig på det mobile apparat. Det skal derfor overvejes og løses, hvordan man i en given selvbetjenings-app beskytter følsomme data, fx gennem kryptering.

Indholdsstyringen kan omfatte en funktion til at præsentere kontekststyret hjælp. Det er hjælpefunktioner, der vejleder brugeren, baseret på det trin i selvbetjeningsforløbet og det sted i en spørgsmål/svar-sekvens, hvor brugeren befinder sig. Dette kan ske gennem hjælpetekster eller andre medier.

Indholdsstyringen kan indeholde en funktion til logning af, hvordan brugeren har brugt brugerfladen, som derefter kan anvendes til analyse. Logningsresultaterne gemmes fortløbende og eksporteres til et eksternt lager efter en nærmere bestemt plan, afhængig af logningens omfang og pladsforbrug. 

Indholdsstyringen anvender:

* Sproghåndtering til at vælge sprog. 
* Funktionalitet til at håndtere de aktive funktionsmuligheder i brugerfladen.
* Integration til at få adgang til brugerprofil eller fagsystem eller fællesoffentlige services.
* Proceshåndtering til at styre en guide eller håndtere en række forskellige veje gennem selvbetjeningsforløbet.

##### Sproghåndtering

Sproghåndtering indeholder den funktionalitet, der skal til, for at et selvbetjeningsforløb kan præsenteres på flere sprog. Det indebærer, at indholdet kan redigeres på flere sprog, og at de forskellige kald af funktionalitet også anvender det valgte sprog såvel som forstår information, der afgives på dette sprog.

Teknologier til sprogoversættelse har gennemgået en stærk udvikling i de senere år, og det vil med flere investeringer bringe maskinel oversættelse frem til et brugbart niveau. Først som hjælp til oversættelse og senere til realtidsoversættelser af faste fraser. Derfor bør sproghåndtering indeholde en service, der leverer automatisk sprogoversættelse. Der vil dog gå nogle år, inden sprogoversættelse til og fra dansk er tilgængelig.

##### Funktionalitet

Set i rammerne af at skabe en god brugerrejse for brugerne skal brugerfladen kunne kalde en række forskellige brugerfladefunktioner. Følgende funktionalitet er af særlig relevans for selvbetjening:

* Afgive informationer gennem en formular
* Levere data og dokumenter til e-mail, Digital Post eller print
* Gennemføre online-chat
* Vise streamet video
* Validere
* Betale
* Godkende
* Kvittere

Funktionalitet kan trække på data for selvbetjeningskonteksten og opdatere denne med brugerens indtastninger og handlinger.   
Funktionalitet anvender integration til at udveksle data med generering af brugerprofiler, fagsystemer og med fællesoffentlige komponenter.  
Funktionalitet kan indgå i procestrin, styret af proceshåndtering.  
Funktionalitet kan inspicere forretningsregler i regelhåndtering.

Hvis de konkrete spørgsmål/svar-forløb i den interaktive afklaring og det interaktive bidrag er simple, fuldstændige og uden megen brug af eksternt hentede data, kan de løses gennem en brugerflade-guide. Simpel og fuldstændig betyder, at der skal være tale om et antal trin, hvor brugeren afgiver informationer og træffer valg, der afslutter et bidrag til at løse selvbetjeningsforløbets opgave. Skal der styres mere komplekse spørgsmål/svar-forløb, og skal der anvendes meget eksternt data, bør man anvende en procesmotor.  
   
I validering kan der ske en formatmæssig validering (fx en dato i korrekt format), en logisk validering (fx en dato, der er realistisk ift. kontekst) og en validering i forhold til kendte registreringer (børns alder kendes og kan bruges til at validere fx skolevalg). Brugerens egen kvalitetssikring af data behandles nedenfor.

##### Proceshåndtering

Proceshåndteringen afvikler spørgsmål/svar-forløb i den interaktive afklaring og det interaktive bidrag. Proceshåndteringen kan også styre kaldene til funktionalitet og eksterne dataressourcer. Med en orkestreringsservice tilrettelægger man spørgsmål/svar og indhentning og opdatering af data, der skal anvendes i selvbetjeningsforløbet. De typiske spørgsmål/svar-forløb er fx at:

* Vise information fra myndigheden, som brugeren efterspørger.
* Opdatere information til myndighedens systemer eller til FO-infrastruktursystemer. 
* Udnytte allerede kendt information om brugeren, som myndigheden har adgang til at vise. 
* Udnytte allerede kendt information om brugeren til at målrette spørgsmål/svar-serien om brugerens erfaring og profil.
* Igangsætte funktionalitet. 

Proceshåndteringen kan anvende en regelhåndtering til at afgøre de valg, som ligger i selvbetjeningsforløbet. 

Proceshåndteringen anvender integration til at hente eller opdatere data fra andre kilder.  
Proceshåndteringen skal føre en log over afviklingen af selvbetjeningsforløbet til brug for analyse og evt. opdatering af brugerprofilen. Det er en forretningsmæssig afgørelse og opgave at udforme denne log. Logningsresultaterne gemmes fortløbende og eksporteres til et eksternt lager efter en nærmere bestemt plan, afhængig af logningens omfang og pladsforbrug samt lovkrav hertil. 

Proceshåndteringen kan læse og opdatere selvbetjeningskonteksten og dermed overdragelseskonteksten.

##### Regelhåndtering

Selvbetjeningsforløbet styres ud fra regler, som er givet af de love og betænkninger, der gælder for den opgave, brugeren skal udføre gennem selvbetjeningsløsningen. Da love og betænkninger ændrer sig løbende, bør reglerne ikke bygges direkte ind i funktioner og processer, men i stedet være tilgængelige, således at funktioner og processer kan spørge på, hvilke regler der er gældende. Derfor bør en regelhåndtering anvendes, således at forretningsreglerne kan gemmes og vedligeholdes af myndighedens medarbejdere, samtidig med at de kan kaldes af funktioner og processer. Hertil er det nødvendigt, at reglerne opmærkes med både en gyldighedsperiode og ikke kun med registrering af opdateringer.

Regelhåndtering bør opbygges, så komponenten både kan anvendes af selvbetjeningsløsningen og et eventuelt fagsystem, så afgørelser træffes på ensartet grundlag, uanset løsning. 

Grundlaget for regelhåndtering kan også dannes gennem resultater af analyser og maskinlæring.

Regelhåndteringen kan læse og opdatere selvbetjeningskonteksten. 

##### Integration

Integration varetager al dataudveksling mellem selvbetjeningsløsningen og datakilder såvel inden for som uden for myndighedens ansvarsområde. Datatransport og datas validitet skal overholde de kvalitetsniveauer, som fastlægges af myndigheden for disse dataudvekslinger. Det er kvalitetsniveauer som disse :

* Karakteristik af de informationer, der overdrages: Den begrebsmodel, der definerer betydningen af de data, der repræsenterer informationen, datas format og volumen, eventuelle metadata tilknyttes.
* Karakteristik af datakilden: validitet, aktualitet, følsomhed, gyldighed og lokation.
* Karakteristik af datatransporten: kommunikationsprotokol, initiativtager til overførslen, løs eller tæt sammenknytning, overførselstid (latency), pålidelighed og integritet, fejlhåndtering og monitering (logning).
* Krav til tidsforløbet: Er selvbetjeningsløsningen afhængig af svar fra datakilden for at kunne gå videre (synkron), eller kan løsningen udføre andre opgaver, mens den venter på svar (asynkron). 

##### Selvbetjeningskontekst

Denne datakomponent lagrer (persisterer) kortvarigt, hvad der beskriver selvbetjeningskonteksten. Det kan fx være:

* Alle informationer, som afgives af brugeren, inklusive dokumenter og andre media.
* Informationer om gennemførte trin i forberedelse, kernen og afrunding.
* Metadata, der karakteriserer det igangværende selvbetjeningsforløb.

Disse data kan være personfølsomme og skal i givet fald beskyttes som sådan. Data skal kun anvendes i det tidsrum, et selvbetjeningsforløb varer, og skal slettes herefter.

##### Overdragelseskontekst

Som det forklares i 10.1.4, er overdragelseskonteksten den del af selvbetjeningskonteksten, som myndigheden må og kan overdrage til det næste selvbetjeningsforløb i rækken, hvis det er nødvendigt for en god betjening af brugeren. Dette kan realiseres på flere måder:

* De to myndigheder kan aftale dataformat og datatransport mellem sig og etablere en en til en-integration. Hvis der er tale om få selvbetjeningsløsninger, der kræver overdragelse, kan dette være en hensigtsmæssig løsning. Hvis en myndighed på den anden side overdrager de samme data til mange, kan det blive en betydelig vedligeholdelses- og driftsopgave for denne myndighed.
* Der kan inden for domæner eller fællesoffentligt aftales en standard for dette dataformat og denne dataoverførsel. Dermed kan en myndighed med mange overdragelser til forskellige myndigheder nøjes med at implementere en integrationssnitflade. Inden for virksomhedsdomænet vil virk.dk facilitere sammenhæng og overdragelsesopgaven.

Der er behov for at indhente erfaringer med overdragelseskontekst, og hvilke måder det kan realiseres på. Disse erfaringer kan betyde ændringer i senere versioner af referencearkitekturen.

Data i overdragelseskontekst kan som i selvbetjeningskontekst være personfølsomme og skal i givet fald beskyttes som sådan, ligesom de skal slettes efter selvbetjeningsforløbets afslutning. Myndigheden skal sikre sig, at der er hjemmel til at anvende brugerens data. Hvis den ikke er til stede, skal brugeren give samtykke til, at data overføres til overdragelseskonteksten.

##### Generering af brugerprofil

Brugerprofilen kan dannes af en analyseplatform, der opsamler oplysninger om brugerens valg og interaktioner med det aktuelle selvbetjeningsforløb og evt. andre selvbetjeningsforløb. Herudfra karakteriseres brugeren med henblik på at tilpasse og målrette information og interaktion med brugerne.

##### Fagsystem

Selvbetjeningsløsninger anvendes ofte til præsentation af information, indsamling af information og godkendelse af information, der skal anvendes i en sagsbehandling, hvortil myndighedens medarbejdere bruger et fagsystem. Disse indgår som leverandør af kendte data og forretningsregler og som modtagere af data. 

Erfaring viser, at det er en fordel at tilrettelægge selvbetjeningsløsningen og fagsystemet i sammenhæng, så de er et spejl af hinanden, selv om de er adskilte systemer. Hvis man gør dette isoleret og hver for sig, kan den ene løsning gøre den anden mere besværlig.

##### Andre fælles komponenter

I Figur 16. Mulige komponenter i selvbetjeningsforløb er der i infrastrukturdelen ikke nævnt de domænekomponenter, som også kan anvendes i selvbetjeningsløsninger. På det kommunale område er det fx Serviceplatformen og støttesystemerne Organisation, Sagsindeks og Ydelsesindeks. På sundhedsområdet er det National Serviceplatform.

Datafordeleren omfatter de grunddata, som nu og i fremtiden bliver tilgængelige i Datafordeleren, fx CPR og CVR.

#### Realiseringsmodeller

Som nævnt i indledning til Del C eksisterer der i markedet mange forskellige formularplatforme og udviklingsrammeværk, som alle i større eller mindre grad indeholder de beskrevne applikationskomponenter i [afsnittet om komponenter](https://fda-preprod.digst.govcloud.dk/node/1100#komponenter). I dette afsnit gives en kort karakteristik af de forskellige muligheder. 

##### Suiter

Der er en lang række udviklingssuiter på markedet, som understøtter en bred vifte af de opgaver, der indgår i virksomheders og myndigheders tilstedeværelse på internettet. En type suite er Content Management System (CMS) med en række funktionelle moduler. En anden type er processtyringsplatforme med tilhørende Content Management-modul.

Fordelene ved suiter er, at de håndterer myndighedens samlede webløsninger og procesunderstøttelse og tilbyder en række funktionaliteter i en sammenhængende pakke. 

Ulemperne i forhold til selvbetjening kan være, at suiterne ikke løser alle opgaver optimalt, og det kan i givet fald betyde lavere kvalitet i selvbetjeningsløsningen. Hvis suiten ikke understøtter snitflader til andre systemer fleksibelt, kan det vanskeliggøre, at myndighedens selvbetjeningsløsning indgår i samspil med andre selvbetjeningsløsninger. Derudover kan suiterne sjældent honorere de skiftende krav til design og funktionalitet uden meget store omkostninger. Ofte kan de slet ikke løse opgaven pga. sammenhæng mellem system og brugergrænseflade. En anden ulempe er, at suiter ofte er samlet gennem opkøb, således at der reelt ikke er tale om en velintegreret samlet løsning.

##### Kommercielle, dedikerede applikationer

Der er en række løsninger på markedet, der er målrettet selvbetjeningsløsninger. Eksempler er blanket- og formularapplikationer.

Fordelen ved dedikerede applikationer er, at de er udviklet med fokus på et specialiseret område og derfor kan have høj kvalitet i forhold til myndighedens krav.

Ulempen er, at myndigheden skal håndtere flere forskellige applikationer og ofte flere forskellige leverandører, samt at myndigheden selv har ansvaret for at skabe de nødvendige integrationer. Nogle dedikerede applikationer kommer dog med integrationer indbygget, fx til CVR og CPR. Derudover kan de dedikerede applikationer sjældent honorere de skiftende krav til design og funktionalitet uden meget store omkostninger. 

##### Skræddersyet udvikling

Til selvbetjeningsløsninger anvendes ofte skræddersyet udvikling, som typisk gennemføres i en udviklingsomgivelse. Udviklerne kan her bygge en løsning med en vifte af delkomponenter til datavalidering, brugerinput, kvittering, processtyring m.m.

Fordelen ved skræddersyet udvikling er en høj grad af tilpasning til det aktuelle selvbetjeningsforløb og dermed en mulighed for at tilbyde en brugerrejse og brugeroplevelse af høj kvalitet.

Ulemperne herved er omkostninger til udvikling og test, der alene hviler på den enkelte myndighed. Samtidig har egenudvikling af denne type en tendens til over tid at blive til meget komplekse og dårligt dokumenterede, hvilket øger vedligeholdelsesomkostningerne.

###### Microservices, smal integration og API management

Gennem de senere år har det internationale marked udviklet en ny type softwarearkitektur og driftsarkitektur, der har været drevet af ønsket om hurtig udvikling og idriftsættelse af funktionalitet og ændringer, udnyttelse af de særlige muligheder, som en cloud-infrastruktur byder på, og håndtering af en eventdrevet arkitektur, der bygger på asynkron kommunikation. Bygger man nyt, enten som egenudvikling eller hos en softwareleverandør, er det værd at overveje, om microservices, smal integration og API management er en vej, man skal gå.

Microservices er services, der opbygges til at implementere de basale kapabiliteter, som en given forretningssituation tilsiger. For disse kapabiliteter konstrueres en applikationskomponent med al logik, beregning og data indkapslet i en snitflade (et Application Programming Interface, API). Sådanne microservices kan idriftsættes uafhængigt af hinanden, hvilket betyder, at ny funktionalitet og nye versioner ikke spænder ben for hinanden. Det betyder også, at de microservices, der belastes hårdt, blot kan dubleres og dermed hurtigt matche det load, de præsenteres for. 

Microservices leverer så sin funktionalitet gennem snitflader , som en brugerfladeimplementering eller en integrationsservice kalder på vegne af en brugerfladeimplementering på en enhed. En sådan integrationsservice skal være meget hurtig og effektiv, hvorfor de eksisterende Enterprise Service-busser (ESB) ikke er anvendelige i de fleste tilfælde. I stedet anvendes en smal integrationsbus, hvor man kun aftaler transportformen og et adresselager. Derefter overlader man til hvert API at foretage alt andet for at realisere dataudvekslingen med den nødvendige kvalitet. Dette kan reduceres til, hvad der lige præcist er nødvendigt for den enkelte microservice og ikke andet. Der findes platforme på markedet, der håndterer dette. 

Med et større antal API’er i spil er der behov for, at man har en styringskomponent, som håndterer, hvilke API’er der kalder hvilke. Dette håndterer sameksistensen af flere versioner af den samme microservice samt de sikkerhedskrav, der gælder, såvel som andre af de kvalitative krav til integrationer. Der findes platforme på markedet, der håndterer dette.

Ulempen er stadig omkostninger til udvikling og test, der alene hviler på den enkelte myndighed.

### Infrastruktur

Infrastruktursynsvinkelen dækker to områder:

* Dels de komponenter og services, som der udvikles og drives fællesoffentligt med henblik på at facilitere interoperabilitet på tværs af blandt andet alle offentlige digitale løsninger.
* Dels services, lager og netværkskomponenter, der implementerer hosting-services og netværksservices. Denne referencearkitektur beskriver ikke komponenter på dette område.

![Figur 17.jpg](C:\Users\B339605\Documents\GitHub\Referencearkitektur-for-selvbetjening\assets\Figur%2017.jpg)

Figur 17. Teknologisk synsvinkel - Infrastruktur

#### Krav til fællesoffentlige komponenter

Selvbetjeningsforløb anvender en række fællesoffentlige komponenter, der enten eksisterer eller er indeholdt i andre af initiativerne i den fællesoffentlige digitaliseringsstrategi. Her beskrives de krav, som denne referencearkitektur stiller til disse komponenter. 

| Komponent                            | Beskrivelse                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| eID, login og signering              | Det er afgørende for selvbetjening, at disse services kan integreres i et selvbetjeningsforløb på en måde, så anvendelsen af dem ikke bliver en barriere for brugeren i forløbet. Derfor er det vigtigt, at den fællesoffentlige referencearkitektur for brugerstyring implementeres, således at der kan oprettes gensidig tillid mellem myndigheder der, hvor en overdragelse finder sted. eID er i 2017 identiske med NemID, senere MitID. Login løses ved NemLog-in.                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Fuldmagt og samtykke                 | Det skal være muligt at anvende fuldmagt i selvbetjeningsløsninger, og selvbetjeningsløsninger har ikke specielle krav i forbindelse med fuldmagt.   <br>Samtykke kan være centralt i forbindelse med at hente data og at overdrage mellem to selvbetjeningsforløb. Samtykke skal her kunne indgå enkelt og forståeligt i selvbetjeningsforløbet.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Datafordeler                         | For at udnytte allerede kendte grunddata skal selvbetjeningsforløb kunne hente grunddata gennem den fællesoffentlige datafordeler. Hvis en bruger gør indsigelse mod grunddata præsenteret, skal selvbetjeningsløsningen have en måde at kommunikere dette og brugerens forslag til de rigtige data til det rette sted.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Overblik sager og ydelser            | I selvbetjeningsforløb kan det være nyttigt at præsentere brugeren for oplysninger om sager, som brugeren er involveret i. Dette gælder også ydelser, som brugeren modtager eller har modtaget, eller om frister, som brugerne skal overholde. På portalen – før og efter et selvbetjeningsforløb eller en selvbetjeningskæde – skal brugeren præsenteres for et globalt overblik over sager. I selvbetjeningsforløbet skal man præsentere det lokale overblik, som er de "sager", man har i netop den kontekst. Disse oplysninger skal kunne trækkes gennem et serviceinterface.                                                                                                                                                                                                                                                                                                                                                              |
| Digital post                         | Borgerens eller virksomhedens digitale postkasse er et vigtigt led i kommunikationen mellem det offentlige og borgere eller virksomheder. Brugen af Digital Post skal derfor kunne indarbejdes sømløst i et selvbetjeningsforløb gennem et serviceinterface, således at selvbetjeningsløsningen kan udnytte Digital Post uden at få en afbrydelse i brugerrejsen.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Katalog over selvbetjeningsforløb    | Der kan i et selvbetjeningsforløb være behov for at give brugeren oplysninger om andre selvbetjeningsmuligheder. Der udvikles og vedligeholdes kataloger over selvbetjeningsløsninger i det offentlige. Det sker i OPIS i borger.dk og i DIA i virk.dk.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Klassifikationer                     | Klassifikationer er en fællesoffentlig komponent, der udstiller snitflader for ontologier, taksonomier, termlister og udfaldsrum, fx KLE og FORM. Der vil over tid udvikles flere nyttige taksonomier eller værdilister mv. Det kunne fx være for livssituationer eller for de statusbetegnelser, som en sag kan gennemløbe. Klassifikationer er standardiseret i 2009, og der pågår et vurderingsarbejde på området. Det skal være muligt for selvbetjening at trække på klassifikationer.                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Kontaktregister                      | Kontaktregistret er en fælleoffentlig komponent under udvikling, som skal indeholde kontaktoplysninger for i første omgang borgere og eventuelt virksomheder. Selvbetjeningsforløb skal kunne trække på dette register såvel som at kunne opdatere det.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Myndighedsregister                   | Myndighedsregistret er en fælleoffentlig komponent, der indeholder informationer om myndighedernes kontaktpunkter. Myndighedsregistret etableres af Digitaliseringsstyrelsen. Selvbetjeningsforløb skal kunne trække på dette register.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Beskedfordeler                       | I forbindelse med genoptagelse og overdragelse kan en selvbetjeningsløsning generere notifikationer (advis) til brugeren, til myndighedens medarbejdere eller andre applikationer. Brugeren kan også i en selvbetjeningsløsning modtage en besked om, at det er tid til at gå videre. Det er beskedfordelerens opgave at kunne modtage besked om hændelser i selvbetjeningsforløb og formidle afsendelse af disse enten på et givent tidspunkt eller baseret på abonnementer fra selvbetjeningsløsninger, fagsystemer eller andre applikationer.                                                                                                                                                                                                                                                                                                                                                                                               |
| Fællesoffentlige integrationsmønstre | For at opfylde målet om, at borgere og virksomheder ikke skal genindtaste allerede kendt information, er udveksling af data centralt for selvbetjening. For at sikre høj kvalitet af disse dataudvekslinger skal man kunne trække på fællesoffentlige mønstre for realisering af integrationer. Disse skal kunne realisere kvalitative krav på forskellige niveauer inden for disse områder:<br><br>*   Karakteristik af de informationer, der overdrages: Den begrebsmodel, der definerer betydningen af de data, der repræsenterer informationen, datas format og volumen, evt. tilknyttet metadata.<br>*   Karakteristik af datakilden: validitet, aktualitet, følsomhed, gyldighed og lokation.<br>*   Karakteristik af datatransporten: kommunikationsprotokol, initiativtager til overførslen, løs eller tæt sammenknytning, overførselstid (latency), fortrolighed, pålidelighed og integritet, fejlhåndtering og monitering (logning). |

#### Krav til snitflader

Referencearkitekturen baseres på standarder og standardsnitflader, hvoraf flere fastlægges i andre referencearkitekturer (se afsnittet om [sammenhæng til den fællesoffentlige rammearkitektur](/node/1100#sammenhng-til-den-fllesoffentlige-rammearkitektur)). Hvilke standarder skal fastlægges i de kommende års arbejde med referencearkitekturer, udvikling af fællesoffentlige komponenter og arbejdet med at omsætte referencearkitekturen til praksis. Der er derfor brug for et arbejde med mere konkrete standarder og vejledninger.

##### Integrationer

Fællesoffentlige integrationsmønstre skal specificere, hvordan de forskellige komponenter kan integreres, fx med henblik på genbrug af eksisterende data og overdragelse mellem forløb. Disse skal kunne realisere kvalitative krav på forskellige niveauer inden for disse områder:

* Karakteristik af de informationer, der overdrages: Den begrebsmodel, der definerer betydningen af de data, der repræsenterer informationen, datas format og volumen, evt. tilknyttet metadata.
* Karakteristik af datakilden: validitet, aktualitet, følsomhed, gyldighed og lokation.
* Karakteristik af datatransporten: kommunikationsprotokol, initiativtager til overførslen, løs eller tæt sammenknytning, overførselstid (latency), pålidelighed, fortrolighed og integritet, fejlhåndtering og monitering (logning).

Der skal være standarder med snitfladespecifikationer for nedenstående snitflader. Disse snitflader omfatter operationer, der kan kaldes eller svare, og det dataformat og den semantik, der udveksles. 

##### Snitflade mellem brugerflade og den underliggende funktionalitet

Offentlige selvbetjeningsløsninger skal anvende de godkendte standarder og snitflader mellem selvbetjeningsløsningens præsentationslag og de funktioner og services, som kan aktiveres i brugerfladen.

##### Snitflader til grunddataregistre

Offentlige selvbetjeningsløsninger skal anvende de godkendte standarder og snitflader til grunddataregistre som CPR, CVR, geodata m.fl.

##### Snitflader til brugerstyring

Offentlige selvbetjeningsløsninger skal anvende de godkendte standarder og snitflader til fællesoffentlig brugerstyring som NemID/MitID og NemLog-in.

##### Snitflader til Digital Post m.m.

Offentlige selvbetjeningsløsninger skal anvende de godkendte standarder og snitflader til fællesoffentlig Digital Post.

##### Snitflader til katalog over selvbetjeningsforløb og selvbetjeningskontekst

Der skal udvikles snitflader, inklusive datastandarder, til katalog over selvbetjeningsforløb og til selvbetjeningskontekst. Der skal fastsættes regler for, under hvilke omstændigheder og hvornår offentlige selvbetjeningsløsninger skal anvende disse.

##### Notifikation (Advis)

Offentlige selvbetjeningsløsninger skal anvende den godkendte fællesoffentlige standard for hændelsesbeskeder.

##### Regelbeskrivelse

Regler, som skal kunne afvikles af et program, skal beskrives entydigt og fuldstændigt. Denne beskrivelse kan udarbejdes både i ”naturligt sprog”, forståelig for jurister, og i et symbolsprog, rettet mod programmører. Offentlige selvbetjeningsløsninger skal anvende de godkendte fællesoffentlige standarder for regelbeskrivelser.

#### Krav til sikkerhed

I [afsnittet Sikkerhed](/node/1100#sikkerhed) er de overordnede krav til sikkerhed beskrevet.

Her beskrives mere detaljerede anvisninger til sikkerhed som følge af, at selvbetjeningsløsninger indgår i samspil med brugerudstyr, andre tjenester og infrastruktur.

Den enkelte tjenesteudbyder vil være afhængig af en række tjenester (fx brugerstyringstjenester som udstedere af akkreditiver, login-tjenester, identitetsbrokere, attributtjenester osv.). Et sikkerhedsbrud i en brugerstyringstjeneste eller forretningstjeneste kan i værste fald påvirke mange tjenester. Det gælder både i forhold til fortrolighed, integritet og tilgængelighed. Dette er et udtryk for det velkendte princip om, at en kæde ikke er stærkere end det svageste led. 

Både risikovurdering og PIA bør afdække krav til sikringsniveauet for de tjenester, som forretningstjenester benytter sig af, fx at brugerne skal autentificeres i henhold til et bestemt sikringsniveau i henhold til NSIS-standarden.

Når der er tale om overdragelse mellem selvbetjeningsforløb, beskriver referencearkitekturen en arkitektur, hvor to eller flere aktører og løsninger skal arbejde sammen om et effektivt og sikkert selvbetjeningsforløb. Dette indebærer en lang række fordele i forhold til fleksibilitet, arbejdsdeling mv., men gør det også mere kompliceret at få et overblik over det samlede sikkerhedsniveau. 

I en distribueret arkitektur er det derfor nødvendigt med fælles rammer for sikkerhed, der definerer roller og ansvar for de forskellige komponenter. Disse spilleregler er grundlaget for tilliden mellem parterne i arkitekturen og bør sikre, at der ikke falder noget mellem to stole. Derudover kan der i den samlede infrastruktur være behov for at have fokus særligt på tværgående aspekter, hvor kompromittering af en tjeneste kan påvirke sikkerheden i en anden tjeneste:

* Når selvbetjeningsløsninger udstiller attributter eller andre stamdata, som bruges af andre selvbetjeningsløsninger til at træffe beslutning om afgørelser eller adgange, er det essentielt at afklare afhængigheder og forudsætninger. Et eksempel kunne være, at sårbarheder i et kildesystem kunne udnyttes til at få adgang til andre systemer (fx at falske data, plantet i et pasregister, udnyttes til at skaffe et eID  i en anden persons navn). Her er det relevant at foretage en tværgående risikovurdering og på forhånd klarlægge kvalitetskrav til de data, der anvendes, således at integriteten af de samlede processer bevares.
* Ved servicekald mellem selvbetjeningsløsninger, der indgår i en samlet forretningsproces, kan der være behov for at etablere og udveksle korrelations-ID'er, således at det bliver muligt ved brug af logfiler at efterforske hændelsesforløb på tværs af tjenester. Hvis hver tjeneste kun ser en lille delmængde af et hændelsesforløb, kan det være vanskeligt at opdage svindel.
* Hvis en tjeneste er afhængig af en anden tjeneste for at kunne fungere, kan manglende tilgængelighed, fx som følge af DDoS-angreb, give kaskadeeffekter på tværs af infrastrukturen.
* Hvis sikkerheden i en tjeneste er afhængig af kontrolmiljøet på slutbrugerens enhed (fx en mobil enhed), kan der være særlige afhængigheder til den part, der udleverer og/eller kontrollerer slutbrugerenhederne.
* Hvis en tjenesteudbyder undlader at implementere log out i tjenesten, betyder det, at en person med adgang til en brugers udstyr kan udnytte en session til at tilgå denne eller en anden tjeneste og fx få adgang til eller ændre data i tjenester og i registreringer vedrørende personen.
* Hvis en tjenesteudbyder indhenter et samtykke hos brugeren, skal det også sikres, at brugeren har mulighed for at tilbagekalde dette samtykke.

Der er her nævnt de vigtigste opmærksomhedspunkter, men man skal altid genbesøge referencearkitektur for brugerstyring og sikre sig, at man kommer omkring alle sikkerhedsovervejelser.

## Bilag A: Tjekliste for vigtige egenskaber

Denne tjekliste kan anvendes af systemejere og leverandører som støtte til at bestille og udvikle produkter og løsninger i forbindelse med digital selvbetjening, som er i overensstemmelse med de vigtigste egenskaber, som defineres i referencearkitekturen.

| Nr.                                                                                                                                    | Arkitekturegenskaber                                                                                                                                                                                                                                                              | Reference                                                                                            | Vurdering |
| -------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | --------- |
| 1                                                                                                                                      | Er det undersøgt ud fra brugerens perspektiv, om løsningen med fordel kan præsenteres mere sammenhængende med andre løsninger?                                                                                                                                                    | [Selvbetjening](/node/1100#beskrivelse-af-emnet-selvbetjening)                                       |           |
| 2                                                                                                                                      | Er der taget stilling til om brugerrejsen skal understøttes af sammenkædning af flere selvbetjeningsforløb?                                                                                                                                                                       | [Brugerrejser](/node/1100#brugerrejser-hvor-der-skal-lses-flere-opgaver)                             |           |
| 3                                                                                                                                      | Er der taget stilling til, om og hvordan der skal ske overdragelse til eller fra andre – og metode herfor?                                                                                                                                                                        | [Brugerrejser](/node/1100#brugerrejser-hvor-der-skal-lses-flere-opgaver)                             |           |
| 4                                                                                                                                      | Er der taget stilling til organisering, ansvarsfordeling, finansiering og fælles arkitektur i forhold til at understøtte eventuelle relevante tværgående brugerrejser?                                                                                                            | [Styrings-rammer](/node/1100#styringsrammer)                                                         |           |
| 5                                                                                                                                      | Er der taget højde for relevante juridiske krav vedr. beskyttelse af persondata, vejledningspligt mv.?                                                                                                                                                                            | [Jura](https://fda-preprod.digst.govcloud.dk/node/1100#jura)                                         |           |
| 6                                                                                                                                      | Er der taget højde for sikkerhed på tværs af de elementer, der indgår i den samlede løsning?                                                                                                                                                                                      | [Sikkerhed](/node/1100#sikkerhed)                                                                    |           |
| 7                                                                                                                                      | Er der taget stilling til hvilke data, der skal indgå i en eventuel overdragelse, og hvordan der sikres hjemmel for dette?                                                                                                                                                        | [Sikkerhed](/node/1100#sikkerhed)                                                                    |           |
| Har projektet gennemgået og aktivt forholdt sig til de seks principper for selvbetjeningsløsninger og de deraf følgende implikationer? |                                                                                                                                                                                                                                                                                   |                                                                                                      |           |
| 8                                                                                                                                      | Princip 1: Brugerne møder i det enkelte selvbetjeningsforløb Forberedelse, Kerne og Afrunding, understøttet af digitale løsninger, der imødekommer brugernes behov                                                                                                                | [Principper](/node/1100#principper)                                                                  |           |
| 9                                                                                                                                      | Princip 2: Brugerne oplever en sammenhængende service også på tværs af myndigheder                                                                                                                                                                                                | [Principper](/node/1100#principper)                                                                  |           |
| 10                                                                                                                                     | Princip 3: Selvbetjeningsløsninger er forståelige, nemme og intuitive at anvende for brugerne.                                                                                                                                                                                    | [Principper](/node/1100#principper)                                                                  |           |
| 11                                                                                                                                     | Princip 4: Brugerne leverer kun information, som det offentlige ikke allerede har                                                                                                                                                                                                 | [Principper](/node/1100#principper)                                                                  |           |
| 12                                                                                                                                     | Princip 5: Brugerne skal kunne se hvilken myndighed, der er ansvarlig for at levere en tjeneste                                                                                                                                                                                   | [Principper](/node/1100#principper)                                                                  |           |
| 13                                                                                                                                     | Princip 6: Myndigheder, der samarbejder om at kæde selvbetjeningsforløb sammen, aftaler opgave- og ansvarsfordeling inden for gældende regler                                                                                                                                     | [Principper](/node/1100#principper)                                                                  |           |
| 14                                                                                                                                     | Anvender projektets dokumentationsmateriale den fællesoffentlige terminologi for de centrale løsningselementer?                                                                                                                                                                   | [Begrebsmodel](https://fda-preprod.digst.govcloud.dk/node/1100#begrebsmodel)                         |           |
| 15                                                                                                                                     | Har projektet gennemtænkt og besluttet relevansen af bestanddelene Forberedelse, Kernen, Afrunding og Overdragelse?                                                                                                                                                               | [Forretningskapabiliteter](https://fda-preprod.digst.govcloud.dk/node/1100#forretningskapabiliteter) |           |
| 16                                                                                                                                     | Har projektet taget stilling til hvilke komponenter, der skal indgå og hvordan de skal realiseres?                                                                                                                                                                                | [Komponenter](/node/1100#komponenter)                                                                |           |
| 17                                                                                                                                     | Har projektet taget højde for eventuelle tværgående udfordringer jf. beskrivelsen i afsnittet, herunder taget stilling til stilling til markedsbaserede formularplatforme og udviklingsrammeværk, som i større eller mindre grad indeholder de beskrevne applikationskomponenter. | [Realiseringsmodeller](https://fda-preprod.digst.govcloud.dk/node/1100#realiseringsmodeller)         |           |
| 18                                                                                                                                     | Anvendes relevante idriftsatte fællesoffentlige infrastrukturkomponenter?                                                                                                                                                                                                         | [Infrastruktur](/node/1100#infrastruktur)                                                            |           |
| 19                                                                                                                                     | Anvendes relevante fællesoffentlige integrationsmønstre og tilhørende standarder.                                                                                                                                                                                                 | [Snitflader](/node/1100#krav-til-snitflader)                                                         |           |
| 20                                                                                                                                     | Overholder løsningen til krav til sikkerhed som følger af samspil med brugerudstyr, andre tjenester og infrastruktur?                                                                                                                                                             | [Sikkerhed](/node/1100#krav-til-sikkerhed)                                                           |           |

## Bilag B: Ordliste

Nedenstående lister forklarer betydningen af de væsentligste ord og begreber, der indgår i den fællesoffentlige referencearkitektur for selvbetjening. For begreber, der indgår i begrebsmodellen, er der her tale om en gentagelse.

| Term                     | Definition                                                                                                                                                                                                            | Note                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Kilde                                     |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| afrunding                | Del af selvbetjeningsforløb, som giver bruger informationer om konsekvenser og anviser det videre forløb.                                                                                                             | En afrunding består af en beskrivelse af den (nye) kontekst, som kernens forløb har bragt brugeren i, hvilke konsekvenser den ændrede kontekst har for brugeren og anvisning af et videre forløb, hvis dette er relevant.<br><br>Alternativ term: rekontekstualisering.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | Referencearkitektur for selvbetjening     |
| bisidder                 | Person, der er til stede ved et møde, en forhandling eller lign. for at hjælpe en af deltagerne, fx som juridisk rådgiver eller som ledsager for en umyndig person.                                                   | Kan i en selvbetjeningskontekst også bistå brugeren med de digitale dele af brugerrejsen.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Den Danske Ordbog                         |
| borger                   | Danske statsborgere, bosiddende i Danmark eller i udlandet, og som har et CPR-nummer.                                                                                                                                 | \-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | \-                                        |
| bruger                   | Person, der gør brug af en it-løsning.                                                                                                                                                                                | \-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | \-                                        |
| brugerprofil             | En samling karakteristiske træk eller egenskaber ved en bruger af offentlige digitale løsninger.                                                                                                                      | Det er muligt gennem analyser af data, genereret af en bruger, at karakterisere denne bruger af selvbetjeningsforløb: Sådanne karakteristika kan anvendes til at tilpasse brugerflade og brugerinteraktion, således at den pågældende brugerprofil nemmere kan udføre selvbetjeningsforløbet.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         | Reference-arkitektur for selvbetjening    |
| brugerrejse              | En brugers oplevelse af et selvbetjeningsforløb eller en selvbetjeningskæde.                                                                                                                                          | Begrebet bruges i denne referencearkitektur, når synsvinklen er brugerens behov og ”den gode brugerrejse”. Der er tale om en mere snæver forståelse af begrebet end den, der normalt gælder inden for servicedesign.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Referencearkitektur for selvbetjening     |
| datavalidering           | Kontrol af, at data overholder krav.                                                                                                                                                                                  | Når brugeren leverer informationer via sit device (apparat), sker der validering af leverede data med henblik på at opnå den bedst mulige datakvalitet.<br><br>De krav, der skal overholdes, er givet af det niveau af sikkerhed og af overholdelse af forretningsregler, som er aktuelt for det konkrete selvbetjeningsforløb.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | \-                                        |
| digital selvbetjening    | Selvbetjening via internettet af en bruger, som anvender en digital brugerflade.                                                                                                                                      | Denne referencearkitektur har fokus på interaktiv, internetbaseret kommunikation i modsætning selvbetjening, fx det at finde varer i et supermarked.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Referencearkitektur for selvbetjening     |
| forberedelse             | Del af et selvbetjeningsforløb, der hjælper brugeren med at afklare forudsætningerne for at løse opgaven i kernen.                                                                                                    | Forberedelsen består af sprogvalg, introduktion, interaktiv afklaring og kan indeholde et interaktivt brugerbidrag.<br><br>Forberedelsen giver informationer til brugeren og kan indsamle informationer. Disse informationer kan lagres i selvbetjeningskonteksten.<br><br>Dele af forberedelse kan ske i en portal, hvor selvbetjeningsforløbet beskrives og noget af eller hele den interaktive afklaring foregår, hvorefter den leder brugeren over til selvbetjeningsforløbets forberedelse eller kernen.                                                                                                                                                                                                                                                                                                                                                         | Referencearkitektur for selvbetjening     |
| fagsystem                | It-løsninger, som varetager særskilte funktioner inden for et eller flere fagområder.                                                                                                                                 | Et fagsystem er typisk bygget til at varetage hele eller dele af sagsbehandlingen inden for et bestemt fagområde.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | Referencearkitektur for selvbetjening     |
| genoptagelse             | Fortsættelse af et afbrudt selvbetjeningsforløb.                                                                                                                                                                      | Informationer, oplyst af brugeren i selvbetjeningsforløbet, lagres, så de er til stede, så længe brugeren ønsker det. Dette gør det muligt at sætte selvbetjeningsforløbet på pause, forlade og genoptage det på et senere tidspunkt med alle informationer intakte.<br><br>Genoptagelse kan implementeres ved, at der eksisterer en kladde, som brugeren kan tage udgangspunkt i, hvis det ønskes.                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | Referencearkitektur for selvbetjening     |
| information              | Viden, der gives videre i en bestemt sammenhæng.                                                                                                                                                                      |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Den Danske Ordbog                         |
| interaktiv afklaring     | Afklaring, som opnås ved, at brugeren gennemgår en serie spørgsmål/svar.                                                                                                                                              | Disse giver brugeren en afklaring af, om vedkommende er på vej ind i det rette selvbetjenings­forløb, afstemmer forventninger om resultater af selvbetjenings­forløbet og forbereder brugeren på, hvad vedkommende eventuelt skal bidrage med.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Referencearkitektur for selvbetjening     |
| interaktivt brugerbidrag | Brugerbidrag, hvor brugeren afgiver eller godkender informationer ved at interagere med en it-løsning.                                                                                                                | Det er gennem det interaktive brugerbidrag, at brugeren afgiver informationer og de handlinger, som opgaven kræver.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | Referencearkitektur for selvbetjening     |
| introduktion             | En indførende, forklarende fremstilling.                                                                                                                                                                              | En introduktion til et selvbetjeningsforløb er tekst, tegninger, billeder eller videoer, der leder brugeren frem til en interaktiv afklaring eller et interaktivt brugerbidrag.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Den Danske Ordbog                         |
| juridisk person          | En retlig enhed, fx et selskab, en forening eller en institution, der i visse henseender kan påtage sig rettigheder og forpligtelser på linje med fysiske personer.                                                   | \-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | denstoredanske.dk                         |
| kerne                    | Del af selvbetjeningsforløb, hvor brugeren gennemfører og løser selvbetjeningsforløbets opgave.                                                                                                                       | En kerne består af interaktive brugerbidrag, hvorigennem brugeren afgiver de nødvendige informationer og accepterer eller godkender selvbetjeningsforløbet. Kernen afsluttes med kvittering og/eller godkendelse og/eller betaling.<br><br>Det er gennem kernen, at såvel bruger som myndighed skal opnå de resultater, informationer og/eller den viden, som blev afstemt i forberedelse. Kernen kræver, at brugeren er logget ind på det sikkerhedsniveau, som udførelsen af opgaven kræver.<br><br>Alternativ term: Gennemførelse.                                                                                                                                                                                                                                                                                                                                 | Referencearkitektur for selvbetjening     |
| kontekstbestemt hjælp    | Hjælp i form af instruktioner til den aktivitet, brugeren er i gang med at udføre.                                                                                                                                    | Selvbetjeningsforløbets brugerflade skal indeholde en kontekstbestemt hjælp, der relaterer sig til det konkrete trin i selvbetjenings­forløbet, som brugeren befinder sig på og hjælper brugeren igennem.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Referencearkitektur for selvbetjening     |
| kvittering               | Dokumentation for de informationer og dokumenter, brugeren har leveret i forberedelse eller kernen.                                                                                                                   | Når opgavens aktiviteter er gennemført, skal brugeren have en eller flere tilbagemeldinger på, hvordan forløbet er gået, og om resultaterne er modtaget og overtaget.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | Referencearkitektur for selvbetjening     |
| livssituation            | Den situation, en bruger står i, som skaber behov for at løse en eller flere opgaver, og som danner afsæt og baggrund for brugerrejsen,                                                                               | Når der sker et skifte i en persons eller en virksomheds livssituation, skal der oftest udføres en række opgaver i relation til offentlig forvaltning og virksomhed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Referencearkitektur for selvbetjening     |
| løsning                  | System, der stilles til rådighed for relevante entiteter, der i henhold til en politik har ret til adgang,                                                                                                            |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | \-                                        |
| medarbejder              | En fysisk person, der arbejder for en virksomhed eller myndighed,                                                                                                                                                     | \-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | \-                                        |
| medbetjener              | én medarbejder i rollen som den, der hjælper brugere med at anvende selvbetjeningsløsninger.                                                                                                                          | \-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | \-                                        |
| myndighed                | Samfundsinstitution, som forvalter og har magtbeføjelser på et bestemt område.                                                                                                                                        | \-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | Den Danske Ordbog                         |
| opgave                   | De handlinger, brugeren har behov for at udføre for realisere brugerrejsens formål.                                                                                                                                   | Eksempler i relation til selvbetjening:<br><br>ansøgning; indberetning; betaling<br><br>En opgave udspringer af en borgers/virksomheds livssituation. Når der sker et skifte i en persons eller en virksomheds livssituation, skal der oftest udføres en række opgaver i relation til offentlig forvaltning og virksomhed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Reference-arkitektur for selvbetjening    |
| overdragelse             | Del af selvbetjeningsforløb, som faciliterer en sammenkædning mellem to selvbetjeningskæder, så dette sker forståeligt og operationelt for brugeren.                                                                  | Overdragelse kan finde sted, når et selvbetjeningsforløb giver anledning til, at der skal løses flere opgaver gennem et eller flere selvbetjeningsforløb, således at forløbene kan kædes sammen i en selvbetjeningskæde.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | Referencearkitektur for selvbetjening     |
| overdragelsesaftale      | En organisatorisk specifikation og aftale om, hvordan et selvbetjeningsforløb tilknyttes et efterfølgende selvbetjeningsforløb.                                                                                       | Overdragelsesaftalen indeholder de forretningsmæssige krav til, med hvilke kvaliteter en overdragelse skal finde sted, herunder krav til datasikkerhed.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | Referencearkitektur for selvbetjening     |
| overdragelses-kontekst   | Den delmængde af en selvbetjeningskontekst, som overdrages ved overdragelse.                                                                                                                                          | Da overdragelse kan ske på tværs af myndigheds- og ressortgrænser, skal der tages stilling til, om kun dele af selvbetjeningskonteksten kan overdrages, og om der skal indhentes samtykke.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | Referencearkitektur for selvbetjening     |
| person                   | én fysisk eller juridisk person.                                                                                                                                                                                      | \-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | \-                                        |
| portal                   | Sted på internettet, som fungerer som indgang til søgning efter bestemte oplysninger, idet det indeholder en stor mængde links til forskellige hjemmesider, som er opdelt efter emne, eller vedrører et bestemt emne. | Eksempler: virk.dk og borger.dk.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | Den Danske Ordbog                         |
| rådgiver                 | En fysisk person, der rådgiver en virksomhed.                                                                                                                                                                         | Rådgiveren kan enten repræsentere virksomheden eller vejlede virksomheden.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            | \-                                        |
| sammenkædning            | En teknisk specifikation og funktion, der knytter et selvbetjeningsforløb til et efterfølgende selvbetjeningsforløb.                                                                                                  | En sammenkædning specificerer tekniske kvalitetskrav til, hvordan to selvbetjeningsforløb kan knyttes sammen teknisk, således at der kan realiseres en hel eller delvis automatisk overdragelse og igangsætning af næste selvbetjeningsopgave.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Referencearkitektur for selvbetjening     |
| selvbetjeningsforløb     | Sammenhængende række af aktiviteter, hvor borgere og virksomheder med en digital brugerflade udfører opgaver i relation til offentlig forvaltning eller virksomhed.                                                   | Et selvbetjeningsforløb består af mindst tre dele: forberedelse, kernen og afrunding.<br><br>Efter en afrunding kan et selvbetjeningsforløb derudover bestå af en overdragelse til et andet selvbetjeningsforløb.<br><br>I selvbetjeningen udfører en bruger opgaver gennem et digitalt interface som fx at ansøge, indberette, indhente information om egne forhold i stedet for, som det var tilfældet tidligere, at løse opgaverne gennem udfyldelse af papirblanketter, indsendelse af breve, telefoniske henvendelser eller personligt fremmøde.<br><br>Når en brugerrejse indebærer gennemførelse af flere selvbetjeningsforløb, som skal kædes sammen, anvendes begrebet ”selvbetjeningskæde”.<br><br>Alternative termer: offentligt digitalt selvbetjeningsforløb, digitalt selvbetjeningsforløb.<br><br>Eksempel: Søge økonomisk friplads til daginstitution | Referencearkitektur for selvbetjening     |
| selvbetjenings-kontekst  | Alle relevante informationer, som er til stede på et givent tidspunkt i et selvbetjeningsforløb.                                                                                                                      | Selvbetjeningskonteksten lagres løbende, så selvbetjeningsforløbet kan genoptages, hvis det afbrydes.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | Referencearkitektur for selvbetjening     |
| selvbetjeningskæde       | Et antal selvbetjeningsforløb, kædet sammen gennem overdragelser, der tilsammen løser de opgaver en bruger i en given livssituation, har behov for at løse gennem selvbetjening.                                      | Selvbetjeningskæder kan være sammensat naturligt, fordi kun en udførelse af flere opgaver samlet set løser en given livssituation. Selvbetjeningskæder kan også have en mere tilfældig sammenhæng, hvor resultatet af en opgave åbner nye muligheder for brugeren.<br><br>Selvbetjeningskæder vil kunne sammenkæde opgaver på tværs af ressortområder.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | Referencearkitektur for selvbetjening     |
| selvbetjenings-løsning   | It-løsning, der implementerer et selvbetjeningsforløb.                                                                                                                                                                | Begrebet bruges i denne referencearkitektur, når der er fokus på den tekniske løsning.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | Referencearkitektur for selvbetjening     |
| servicedesign            | En proces, der fokuserer på at skabe optimale serviceoplevelser ved at anlægge et helhedssyn på alle involverede aktører, deres interaktioner og de materialer og infrastrukturer, som de anvender i processen.       | Involverer ofte brugen af brugerrejse-kortlægning, som fortæller historien om forskellige brugeres interaktion med og omkring produktet for dermed at give dybere indsigter.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | Interaction-design foundation<br><br>.org |
| servicegodkendelse       | Accept af at de interaktive brugerbidrag er i overensstemmelse med brugerens ønsker og behov og den accept af de betingelser hvorunder brugerbidraget er afgivet.                                                     | Det kan være en aktivitet i kernen, at brugeren skal bekræfte læst information, de oplysninger, der er indtastet, information og valg, som brugeren har afgivet, informationer hentet fra andre registre, eller de betingelser (fx Tro og love, samtykker etc.), som afgivelsen af oplysningerne sker under, En servicegodkendelse kan dokumenteres med forskellig styrke og stærkest gennem en digital signering.                                                                                                                                                                                                                                                                                                                                                                                                                                                    | Referencearkitektur for selvbetjening     |
| sprogvalg                | Valg af sprog, der læses, skrives eller tales på.                                                                                                                                                                     | Her vælges det sprog, som selvbetjeningsforløbet vil blive formidlet i. Ønsker man at adressere brugerne ud fra deres profiler, kan der vælges mellem forskellige persona, som man har defineret.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | Referencearkitektur for selvbetjening     |
| tjeneste                 | En tjeneste er en leverance til en bruger af en velbeskreven, sammenhængende funktionalitet, som løser en eller flere opgaver for brugeren.                                                                           | En tjeneste kan leveres af personer eller teknologi eller en kombination af personer og teknologi. En tjeneste kan i udførelsen af sin funktionalitet trække på andre tjenester.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | Referencearkitektur for selvbetjening     |
| udlænding                | Udenlandske statsborgere, bosiddende i Danmark eller i udlandet.                                                                                                                                                      | \-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | .                                         |
| brugervejledning         | Vejledning i, hvordan man gennemfører brugerrejsen, herunder anvender selvbetjeningsløsningen.                                                                                                                        | Selvbetjeningsforløbet støttes af vejledning til brugerne om at gennemføre den brugerrejse, som selvbetjeningen repræsenterer. Det er materiale med råd, retningslinjer og instruktioner i at gennemføre selvbetje­nings­forløbet.<br><br>Brugervejledninger kan være målrettet brugerprofiler.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Referencearkitektur for selvbetjening     |
| videre forløb            | Del af afrunding, som beskriver, hvad brugeren kan forvente og skal gøre i den videre behandling af sagen.                                                                                                            | Del af afrundingen, der i tekst, tegninger, billeder eller videoer beskriver for brugeren, hvad der sker som resultat af brugerens bidrag.<br><br>Her beskrives, hvem den ansvarlige myndighed er, hvad brugeren skal gøre, hvad myndigheden gør, og hvilke tidsforløb brugeren kan forvente.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         | Referencearkitektur for selvbetjening     |
| virksomhed               | En registreret organisation med et forretningsformål.                                                                                                                                                                 | Virksomheder er registreret i CVR. CVR omfatter også offentlige organisationer, som derfor også kan være ”virksomheder”.<br><br>Optræder gennem følgende roller i virksomheden: ejer, medarbejder eller supporter. Dertil kan virksomheder optræde som rådgiver.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |                                           |

## Bilag C: Oversigt over kilder og baggrundsmateriale

Nedenstående liste viser det baggrundsmateriale, der indgår i udarbejdelsen af den tværoffentlige referencearkitektur for selvbetjening.

| Kilde                                                  | Materiale                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Digitaliseringsstyrelsen                               | Vejledning i vurdering af offentlige it-projekters potentielle konsekvenser for privatlivet; maj 2013. [http://www.digst.dk/informationssikkerhed/Konsekvensvurdering-for-privatlivet](https://digst.dk/media/13729/guide-til-konsekvensvurdering-af-privatlivsbeskyttelsen_ver3.pdf)                                                                                                                             |
| Digitaliseringsstyrelsen og Center for Cybersikkerhed  | Anbefalinger til styrkelse af sikkerheden i statens outsourcede it-drift; august 2014. [https://www.ft.dk/samling/20131/almdel/REU/bilag/353/1394280.pdf](https://www.ft.dk/samling/20131/almdel/REU/bilag/353/1394280.pdf)                                                                                                                                                                                       |
| EU-Kommissionen                                        | EU’s databeskyttelsesforordning (persondataforordning); maj 2018. [http://eur-lex.europa.eu/legal-content/DA/TXT/PDF/?uri=CELEX:32016R0679&from=DA](http://eur-lex.europa.eu/legal-content/DA/TXT/PDF/?uri=CELEX:32016R0679&from=DA)                                                                                                                                                                              |
| EU-Kommissionen                                        | Europa-Parlamentets og Rådets direktiv (EU) 2016/2102 af 26. oktober 2016 om tilgængeligheden af offentlige organers websteder og mobilapplikationer (EØS-relevant tekst); oktober 2016. [http://eur-lex.europa.eu/legal-content/DA/TXT/?qid=1481622494924&uri=CELEX:32016L2102](http://eur-lex.europa.eu/legal-content/DA/TXT/?qid=1481622494924&uri=CELEX:32016L2102)                                           |
| Europa-Kommissionen                                    | EU-wide digital Once-Only Principle for citizens and businesses: Policy options and their impacts; april 2009. [https://ec.europa.eu/digital-single-market/en/news/eu-wide-digital-once-only-principle-citizens-and-businesses-policy-options-and-their-impacts](https://ec.europa.eu/digital-single-market/en/news/eu-wide-digital-once-only-principle-citizens-and-businesses-policy-options-and-their-impacts) |
| Den fællesoffentlige digitaliseringsstrategi 2016-2020 | [https://digst.dk/media/12810/faellesoffentlige-digitaliseringsstrategi-2016-2020-dobbeltopsl.pdf](https://digst.dk/media/12810/faellesoffentlige-digitaliseringsstrategi-2016-2020-dobbeltopsl.pdf)                                                                                                                                                                                                              |
| Hvidbog om fællesoffentlig digital arkitektur          | [https://arkitektur.digst.dk/node/241](/node/241)                                                                                                                                                                                                                                                                                                                                                                 |
| Regeringen                                             | National strategi for cyber- og informationssikkerhed; december 2014. [https://digst.dk/media/13813/national-strategi-for-cyber-og-informationssikkerhed-2015-2016.pdf](https://digst.dk/media/13813/national-strategi-for-cyber-og-informationssikkerhed-2015-2016.pdf)                                                                                                                                          |
| Regeringen                                             | Sammenhængsreformen: Borgeren først - en mere sammenhængende offentlig sektor; april 2017. [https://fm.dk/udgivelser/2017/april/sammenhaengsreform-borgeren-foerst-en-mere-sammenhaengende-offentlig-sektor/](https://fm.dk/udgivelser/2017/april/sammenhaengsreform-borgeren-foerst-en-mere-sammenhaengende-offentlig-sektor/)                                                                                   |
| Regeringen, KL og Danske Regioner                      | Et stærkere mere trygt digitalt samfund: Den fællesoffentlige digitaliseringsstrategi 2016-2020; maj 2016. [https://digst.dk/media/12810/faellesoffentlige-digitaliseringsstrategi-2016-2020-dobbeltopsl.pdf](https://digst.dk/media/12810/faellesoffentlige-digitaliseringsstrategi-2016-2020-dobbeltopsl.pdf)                                                                                                   |
| Regeringen, KL og Danske Regioner                      | Den fællesoffentlige rammearkitektur; [https://arkitektur.digst.dk/node/17/](https://arkitektur.digst.dk/node/17/)                                                                                                                                                                                                                                                                                                |
| Regeringen, KL og Danske Regioner                      | Den digitalt sammenhængende offentlige sektor: Hvidbog om fællesoffentlig digital arkitektur; juni 2017. [https://arkitektur.digst.dk/node/241](/node/241)                                                                                                                                                                                                                                                        |
| Regeringen, KL og Danske Regioner                      | Referencearkitektur for: Overblik over egne sager, Tværgående processer, Deling af data og dokumenter; Under udarbejdelse. [https://arkitektur.digst.dk/referencearkitekturer](/node/122/)                                                                                                                                                                                                                        |
| Regeringen, KL og Danske Regioner                      | Referencearkitektur for Brugerstyring; april 2017. [https://arkitektur.digst.dk/node/123/](/node/123/)                                                                                                                                                                                                                                                                                                            |
| Rigsrevisionen                                         | Beretning om brugervenligheden af offentlig digital selvbetjening for virksomheder; november 2015. [https://rigsrevisionen.dk/revisionssager-arkiv/2015/nov/beretning-om-brugervenligheden-af-offentlig-digital-selvbetjening-for-virksomheder](https://rigsrevisionen.dk/revisionssager-arkiv/2015/nov/beretning-om-brugervenligheden-af-offentlig-digital-selvbetjening-for-virksomheder)                       |
| Justitsministeriet                                     | Bekendtgørelse om sikkerhedsforanstaltninger til beskyttelse af personoplysninger, som behandles for den offentlige forvaltning; marts 2001. [https://www.retsinformation.dk/Forms/R0710.aspx?id=842](https://www.retsinformation.dk/Forms/R0710.aspx?id=842)                                                                                                                                                     |
| Justitsministeriet                                     | Forvaltningsloven; april 2014. [https://www.retsinformation.dk/forms/r0710.aspx?id=161411](https://www.retsinformation.dk/forms/r0710.aspx?id=161411)                                                                                                                                                                                                                                                             |
| Regeringen                                             | Lov om behandling af personoplysninger; maj 2000. [https://www.retsinformation.dk/forms/r0710.aspx?id=828](https://www.retsinformation.dk/forms/r0710.aspx?id=828)                                                                                                                                                                                                                                                |
| Styrelsen for Arbejdsmarked og Rekruttering            | Bekendtgørelse om obligatorisk digital selvbetjening vedrørende ansøgninger og meddelelser mv. om sociale ydelser mv.; november 2015. [https://www.retsinformation.dk/Forms/R0710.aspx?id=175675](https://www.retsinformation.dk/Forms/R0710.aspx?id=175675)                                                                                                                                                      |

## Fodnoter

[\[1\]](#_ednref1) Myndighedernes virksomhedsrettede løsninger præsenteres/integreres på Virk, således at de fremstår som en del af Virk.

[\[2\]](#_ednref2) Rigsrevisionen (2015): "Beretning om brugervenligheden af offentlig digital selvbetjening for virksomheder" [https://www.rigsrevisionen.dk/revisionssager-arkiv/2015/nov/beretning-om...](https://www.rigsrevisionen.dk/revisionssager-arkiv/2015/nov/beretning-om-brugervenligheden-af-offentlig-digital-selvbetjening-for-virksomheder)

[\[3\]](#_ednref3) Servicedesign er tilrettelæggelse af de berøringsflader, der er mellem udbyder og slutbruger, fysiske som digitale, med udgangspunkt i brugerens perspektiv. Resultatet af servicedesign er den faktiske oplevelse af forbedring af [serviceniveauet](https://da.wikipedia.org/w/index.php?title=Serviceniveau&action=edit&redlink=1) hos slutbrugeren.

[\[4\]](#_ednref4) Folketinget har vedtaget første samlelov lov nr. 558 af 18. juni 2012, anden samlelov lov nr. 622 af 12. juni 2013, tredje samlelov lov nr. 552 af 2. juni 2014 og fjerde samlelov lov nr. 742 af 1. juni 2015. [https://digst.dk/strategier/den-faellesoffentlige-digitaliseringsstrateg...](https://digst.dk/strategier/den-faellesoffentlige-digitaliseringsstrategi/tidligere-strategier/digitaliseringsstrategien-2011-2015/lovgivning-om-obligatorisk-digital-selvbetjening/)

[\[5\]](#_ednref5) Pr. 2017 NemID senere MitID

[\[6\]](#_ednref6) [http://arkitekturguiden.digitaliser.dk/principper/10](http://arkitekturguiden.digitaliser.dk/principper/10-overordnede-principper)[\-o](http://arkitekturguiden.digitaliser.dk/principper/10-overordnede-principper)[verordnede](http://arkitekturguiden.digitaliser.dk/principper/10-overordnede-principper)[\-](http://arkitekturguiden.digitaliser.dk/principper/10-overordnede-principper)[principper](http://arkitekturguiden.digitaliser.dk/principper/10-overordnede-principper)

[\[7\]](#_ednref7) [https://arkitektur.digst.dk/node/241](https://arkitektur.digst.dk/node/241)

[\[8\]](#_ednref8) Se også referencearkitektur for deling af data og dokumenter (2018) med fællesoffentlige integrationsmønstre.

[\[9\]](#_ednref9) I Afsnit 7.1 ovenfor er der redegjort for de juridiske overvejelser, der er nødvendige. Juridiske overvejelser kan også omfatte muligheden for at gennem ændret lovgivning at skabe hjemmel til at anvende data.

[\[10\]](#_ednref10) Se fx [https://fm.dk/udgivelser/2017/april/sammenhaengsreform-borgeren-foerst-en-mere-sammenhaengende-offentlig-sektor/](https://fm.dk/udgivelser/2017/april/sammenhaengsreform-borgeren-foerst-en-mere-sammenhaengende-offentlig-sektor/)

[\[11\]](#_ednref11) Et eksempel er nystartede fødevarevirksomheder, der også vil servere alkohol. Fra Rigsrevisionens beretning [https://rigsrevisionen.dk/revisionssager-arkiv/2015/nov/beretning-om-bru...](https://rigsrevisionen.dk/revisionssager-arkiv/2015/nov/beretning-om-brugervenligheden-af-offentlig-digital-selvbetjening-for-virksomheder)

[\[12\]](#_ednref12) Som i 2017 fx kan ske ved brug af beskedfordeler i KOMBIT-støttesystemer eller ved brug af Digital Post,

[\[13\]](#_ednref13) Der skal gennemføres pilotprojekter i 2018, som skal afklare, hvilke informationer der er nyttige at overføre en overdragelse,

[\[14\]](#_ednref14) En skabelon for udarbejdelse af en overdragelsesaftale er planlagt udarbejdet af Digitaliseringsstyrelsen til levering i 2018.

[\[15\]](#_ednref15) Vejledning i integrationsmønstre med forskellige kvalitetsniveauer er planlagt udarbejdet af Digitaliseringsstyrelsen til levering i 2018.

[\[16\]](#_ednref16) Pr. 2017 NemID senere MitID.

[\[17\]](#_ednref17) Vejledning i integrationsmønstre med forskellige kvalitetsniveauer er planlagt udarbejdet af Digitaliseringsstyrelsen til levering i 2017.

[\[18\]](#_ednref18) Microservices kan også anvendes sammen med synkrone services, men en hurtig smal asynkron servicebus byder på en række fordele.

[\[19\]](#_ednref19) Dertil vil initiativ 7.1 til 7.4 i den fællesoffentlige digitaliseringsstrategi bidrage med opdatering og videreudvikling af redskaberne på sikkerhedsområdet.

[\[20\]](#_ednref20) Pr. 2017 NemID senere MitID.

[\[21\]](#_ednref21) Vejledning i integrationsmønstre med forskellige kvalitetsniveauer er planlagt udarbejdet af Digitaliseringsstyrelsen til levering i 2017.
