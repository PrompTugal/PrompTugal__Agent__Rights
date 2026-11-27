# P18 stage 3: rulings for 131 source hosts

Read 2026-11-27 by cl-6.rights@PrompTugal.dinis from each site's own pages (robots first, then home page, then the terms or legal link in the site's own anchors, same host only). Courtesy agent string, about one request per 1.2 s. No challenge, login or refusal was worked round (R13). No agent accepts terms.

Meanings: READ OK (facts only) = names, dates, amounts with source link and read date, no text or images copied. NEEDS DINIS = a restriction or a refusal that only Dinis can accept or lift. NEVER = the terms ban what we would do. NEEDS A PERSON = a gap I could not read; a person checks in a browser. A keyword scan can mis-pick a link: those hosts are ruled "no terms found", not as a clean pass.

Full list: `p18-stage3-rulings.csv`. Together with stages 1 and 2, this covers the 173 hosts, except those still marked UNCHECKED in stage 1.

## Totals

- READ OK (facts only): 96
- NEEDS DINIS: 20
- NEVER: 7
- NEEDS A PERSON: 6
- READ OK (public pages only): 2

## NEVER

- `vestbee.com`: terms prohibit data scraping and republishing website content ([terms](https://vestbee.com/terms))
- `www.forbespt.com`: terms forbid copying, storing, reproducing, commercial use ([terms](https://www.forbespt.com/termos-e-condicoes/))
- `www.diariodominho.pt`: terms forbid copying, reproduction and use of texts and photographs ([terms](https://www.diariodominho.pt/termos-e-condicoes))
- `www.diarioleiria.pt`: subscriber content may not be copied or distributed ([terms](https://www.diarioleiria.pt/termos-condicoes))
- `www.vestbee.com`: terms prohibit data scraping and republishing website content ([terms](https://www.vestbee.com/terms))
- `registo.justica.gov.pt`: terms ban web scraping and automated extraction ([terms](https://registo.justica.gov.pt/Termos-e-Condicoes))
- `www.diarioviseu.pt`: subscriber content may not be copied or distributed ([terms](https://www.diarioviseu.pt/termos-condicoes))

## NEEDS DINIS

- `www.startupbraga.com`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://www.startupbraga.com/termsandconditions))
- `www.portugalglobal.pt`: reuse allowed with source; the portal says its information may not be sold, so no use on a billed page without Dinis ([terms](https://www.portugalglobal.pt/termos-e-condicoes/))
- `www.portugalventures.pt`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://www.portugalventures.pt/termos-e-condicoes-de-utilizacao/))
- `dealroom.co`: data vendor; no terms page found; asking Dinis before any use
- `www.essential-business.pt`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://www.essential-business.pt/terms-and-conditions/))
- `www.bpfomento.pt`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://www.bpfomento.pt/pt/aviso-legal/))
- `startupgenome.com`: data vendor; no terms page found; asking Dinis before any use
- `www.edp.com`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://www.edp.com/en/terms-and-conditions-use))
- `www.cuatrecasas.com`: robots.txt disallows the home page for Claude; not read and not worked round (R13)
- `www.iapmei.pt`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://www.iapmei.pt/pt/footer/termos-e-condicoes/))
- `www.compete2030.gov.pt`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://www.compete2030.gov.pt/termos-e-condicoes/))
- `funding.tech.eu`: data vendor; no terms page found; asking Dinis before any use
- `www.londonstockexchange.com`: data vendor; no terms page found; asking Dinis before any use
- `www.connectventures.co`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://www.connectventures.co/cookies-policy))
- `www.kcl.ac.uk`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://www.kcl.ac.uk/terms))
- `www.roehampton.ac.uk`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://www.roehampton.ac.uk/site/terms-and-conditions/))
- `fintech.global`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://fintech.global/term-conditions/))
- `sapo.pt`: robots.txt disallows the home page for Claude; not read and not worked round (R13)
- `www.uevora.pt`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://www.uevora.pt/termos-e-condicoes-e-politica-de-privacidade/politica-de-privacidade))
- `www.dig-in.io`: terms restrict copying or commercial use; see the clause at the terms page ([terms](https://www.dig-in.io/terms))

## NEEDS A PERSON

- `www.jornaldenegocios.pt`: gap: home page not readable (HTTP 000 or challenge): a gap
- `www.cm-viana-castelo.pt`: gap: terms page not readable (HTTP 000): a gap ([terms](https://www.cm-viana-castelo.pt/areas-de-atividade/comunicacao/editais-e-avisos-em-vigor))
- `www.ipcb.pt`: gap: terms page not readable (HTTP 000): a gap ([terms](https://www.ipcb.pt/estudar/cursos/licenciatura/))
- `www.euacc.ai`: gap: home page not readable (HTTP 429 or challenge): a gap
- `www.cm-leiria.pt`: gap: home page not readable (HTTP 000 or challenge): a gap
- `vitebtestbed.com`: gap: home page not readable (HTTP 200 or challenge): a gap

## READ OK (public pages only)

- `transparencia.gov.pt`: public data, reuse invited ([terms](https://transparencia.gov.pt/termos-e-condicoes))
- `digital-strategy.ec.europa.eu`: EU legal notice allows reuse with attribution ([terms](https://digital-strategy.ec.europa.eu/en/pages/legal-notice#ecl-inpage-km0gezfs))

## READ OK (facts only)

96 hosts; reasons in the CSV. Two groups: terms page read with only copyright-reserved or own-use wording, and no terms found on the site's own pages.

## Caveats

- Terms in Portuguese were scanned for ban wording near copy, commercial and scrape words, then the flagged clauses read by me. A clause I missed is possible; the ruling is only as good as the scan.
- "Facts only" is not licence to show a table, a ranking or a database extract: a site's compiled data may carry database rights. Check per use.
- Four data vendors without a terms page are held for Dinis: dealroom.co, startupgenome.com, www.londonstockexchange.com, funding.tech.eu.
