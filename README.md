# Tree School Contest - Prova Codice

Ciao a tutti e benvenuti alla seconda prova del Contest Tree School!

Questo è un chat Client sviluppato in React utilizzando le API di [Rocket.Chat](https://rocket.chat/).

## Per iniziare

## Step 0
Aprite il terminale e seguite i passaggi qui sotto.

```
git clone [inserire url comunicato dai docenti] contest-tree
```

```
cd contest-tree
```

```
npm install
```

```
npm start
```

Nel Contest dovrete implementare la UI come da Grafica (che trovate qui sotto) e poi la integreremo con le API di Rocket.Chat.

![ui-implementation](./assets/ui-implementation.png)

Il Contest è diviso in 6 Step, 20 minuti per step.
Al termine dei 20 minuti vi verrà comunicata la soluzione dello step, indipendentemente da dove siete arrivati.
Questo vi permetterà di andare avanti anche se non avete completato lo step precedente.

# IMPORTANTE
Quando i docenti ve lo comunicano (al termine degli slot da 20 minuti) dovrete pushare il codice su una nuova branch, questi sono i passaggi da seguire:

Aprite il terminale e cambiate cartella fino a trovarvi alla path corretta

```
cd /path/to/contest-tree
```

```
git checkout -b [step-numerostep]
```

```
git add *
```

```
git commit -m "Inserite un commento descrittivo di quello che avete fatto nello step"
```

```
git push --set-upstream origin [step-numerostep]
```



# Inizia la prova!

## Step 1

- Impostare come endpoint delle API il seguente url: `http://51.15.43.78:3000/`


## Step 2

- Implementare la ricerca degli utenti utilizzando il componente SearchBox
  (occhio! La SearchBox è in realtà un form, e che fanno i form al submit? Refreshano la pagina!)

## Step 3

- Implementare la lista degli utenti utilizzando il componente ChatPreview

## Step 4

- Implementare l'ordinamento della lista utenti

## Step 5

- Implementare la SendBox (trovate i riferimenti alla chiamata API necessaria qui sotto e sopra la funzione sendMessage, occhio al parsing della risposta!)

## Step 6

- Implementare la lista di messaggi nella chat con un utente (componente Message)


## API

Le reference alle API di rocket.chat che potrebbero interessarvi:

### Login Utente

- api/v1/login - [documentazione](https://rocket.chat/docs/developer-guides/rest-api/authentication/login/)

### Info Utente

- api/v1/me - [documentazione](https://rocket.chat/docs/developer-guides/rest-api/authentication/me/)

### Lista Utenti

- api/v1/users.list - [documentazione](https://rocket.chat/docs/developer-guides/rest-api/users/list/)

### Invio Messaggio

- api/v1/chat.postMessage - [documentazione](https://rocket.chat/docs/developer-guides/rest-api/chat/postmessage/)

### Lista Messaggi Diretti

- api/v1/im.messages - [documentazione](https://rocket.chat/docs/developer-guides/rest-api/im/messages/)

### Creazione Messaggio Diretto con un Utente

- api/v1/im.create - [documentazione](https://rocket.chat/docs/developer-guides/rest-api/im/create/)

