<h1>Descrizione</h1>
Web/App per la palestra che offre schede di allenamento personalizzate in base agli obiettivi e all'esperienza dell'utente, integrate con piani alimentari personalizzati per ottimizzare i risultati. Gli utenti possono accedere a video esecuzioni e 
interfacciarsi con gli eventuali coach per imparare la corretta tecnica degli esercizi e monitorare i progressi + video editati indirizzati al marketing della web/app.

<h1>Problema</h1>
Sapere come comportarsi per ottenere i massimi
risultati del proprio corpo è spesso complesso. Con BeastMode
è tutto più semplice

<h1>Target</h1>
Persone che non hanno
idea di come proseguire
il proprio percorso in
palestra, vedendo pochi
risultati o addirittura nulli

<h1>Competitors</h1>
BltDifferent
FitBod
Tracked

<h1>Tagline</h1>
Ottieni il corpo dei tuoi sogni

<h1>Tecnologie</h1>
Mobile app

<h1>UML Use Case</h1>

// Sweet Use Case Diagram
// ----------------------

// Actors
[Customer]-(Register / Login)
[Customer]-(Manage Profile)
[Customer]-(View Workout Plans)
[Customer]-(Purchase Subscription)
[Customer]-(Access Personal Trainer)
[Customer]-(Access Nutritionist)
[Customer]-(Receive Personalized Workout Plan)
[Customer]-(Receive Nutrition Plan)

[Trainer]-(Create Workout Plans)
[Nutritionist]-(Create Nutrition Plans)
[Admin]-(Manage Content and Subscriptions)

// Include / Extend relationships
(Access Personal Trainer)>(Receive Personalized Workout Plan)   // include
(Access Nutritionist)>(Receive Nutrition Plan)                  // include

(Purchase Subscription)<(Access Personal Trainer)               // extend
(Purchase Subscription)<(Access Nutritionist)                   // extend

// Inheritance (specialized actors)
[Trainer]^[Customer]
[Nutritionist]^[Customer]

// Notes
(Access Personal Trainer)-.-[note: Requires active subscription]
(Access Nutritionist)-.-[note: Available only with nutrition plan]
