# GESTIONE DEL PARAMETRO COLLECT_EMAIL (SCRIPT DI CONFIGURAZIONE DI CLERK)



L'impostazione del parametro "collect_email" nello script di
configurazione consente di decidere se Clerk dovrà o meno raccogliere in
maniera automatica, durante la sessione di navigazione, l'indirizzo
e-mail dell'utente. Nello specifico utilizzando l'impostazione

- *collect_email: false*

> Clerk non raccoglierà in maniera automatica l'indirizzo email
> dell'utente.
>
> **ATTENZIONE**: considerando che questa è l'opzione di default, nel
> momento in cui si dovesse impostare lo script di configurazione di
> Clerk senza indicare in maniera esplicita un valore per il parametro
> in oggetto questo equivarrà di fatto all'impostazione *collect_email:
> false*

- *collect_email: true*

> Clerk raccoglierà in maniera automatica, durante la sessione di
> navigazione l'indirizzo email del cliente. In particolare attivando
> questa impostazione Clerk.js monitorerà tutti i campi di input
> presenti all'interno del sito e nel momento in cui l'utente dovesse
> inserire in uno di essi (es. in fase di login all'interno del campo
> 'username') il suo indirizzo mail, questo verrà automaticamente
> inviato a Clerk con una chiamata all'endpoint 'log/email'

Il fatto di raccogliere, durante una sessione di navigazione,
l'indirizzo email dell'utente può portare ovviamente diversi vantaggi
tra cui ad esempio:

- **Consente di associare le attività anonime ad un utente conosciuto**.

> Quando l'utente si identifica (effettuando ad esempio il login al sito
> mediante il suo indirizzo email) le attività precedentemente tracciate
> da Clerk (click, ricerche, acquisti ...) saranno associate ad un
> utente conosciuto

- **Migliora la personalizzazione delle Raccomandazioni**

> Dopo aver raccolto l'email, Clerk può mostrare consigli più precisi,
> basati anche sulla cronologia ordini o preferenze passate associate a
> quell'indirizzo

- **Alimenta i moduli Email e Audience**

> ...

Va da sé quindi che il consiglio è ovviamente quello di impostare nello
script di configurazione di Clerk l'opzione *collect_email: true*

*\<!\-- Start of Clerk.io E-commerce Personalisation tool - www.clerk.io
\--\>*

*\<script type=\"text/javascript\"\>*

*(function(w,d){*

*var
e=d.createElement(\'script\');e.type=\'text/javascript\';e.async=true;*

*e.src=\'https://cdn.clerk.io/clerk.js\';*

*var
s=d.getElementsByTagName(\'script\')\[0\];s.parentNode.insertBefore(e,s);*

*w.\_\_clerk_q=w.\_\_clerk_q\|\|\[\];w.Clerk=w.Clerk\|\|function(){w.\_\_clerk_q.push(arguments)};*

*})(window,document);*

*Clerk(\'config\', {*

*key: \'{clerk_public_key}\',*

***collect_email: true**,*

*{clerk_visitor_type}*

*});*

*\</script\>*

*\<!\-- End of Clerk.io E-commerce Personalisation tool - www.clerk.io
\--\>*

( <https://docs.clerk.io/docs/clerkjs-configuration> ).

Dal punto di vista del GDPR occorre invece considerare che **se l'email
viene utilizzata esclusivamente per finalità connesse all'esecuzione del
contratto** (es. personalizzazioni post-ordine, notifiche ...) non serve
ulteriore consenso per cui, in queste condizioni, si può tranquillamente
impostare nello script di configurazione il parametro collect_email
sull'opzione true.

Va comunque indicato in Privacy Policy, se ritenuto rilevante, che
l'email dell'utente sarà utilizzata anche a fini di personalizzazione
dei contenuti del sito

**ATTENZIONE!** **nel caso in cui l'email raccolta da Clerk dovesse
essere utilizzata anche per finalità marketing** (newsletter,
retargeting ...) **sarà invece necessario richiedere un consenso
esplicito e separato** (es. mediante in check di iscrizione alla
newsletter)

**Il consiglio, in ogni caso, è sempre quello di verificare direttamente
con il supporto Clerk o con il proprio DPO che la soluzione adottata sia
effettivamente conforme a quanto richiesto dal GDPR**

