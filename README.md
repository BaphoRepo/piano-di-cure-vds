# Piano di Cure VDS

Applicazione web di I Viaggi Del Sorriso per comporre il piano di cure del paziente e
esportarlo in PDF A4 (4 pagine, oppure solo copertina e preventivo) o in Excel.

- Pagina unica `index.html`, pubblicata con GitHub Pages.
- Accesso con l'account dello studio (Supabase Auth, progetto `vds-crm`).
- Preventivi e listino salvati nelle tabelle `vds_preventivi` e `vds_listino`,
  protette da Row Level Security: solo l'account autorizzato può leggerle o modificarle.

La chiave Supabase contenuta nella pagina è quella pubblica ("publishable"): da sola non dà accesso ai dati.
