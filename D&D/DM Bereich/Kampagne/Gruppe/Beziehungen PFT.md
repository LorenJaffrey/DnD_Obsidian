``` mermaid
flowchart LR
Aranon
Drogan
Lucian
Jon
Niptac

Aranons_Stamm{{Aranons Stamm}}

Jon -- Buddys --- Niptac
Drogan -- Kriegskameraden --- Jon
Aranon -- lebte in ---> Aranons_Stamm
Lucian -- half bei Zerstörung von ---> Aranons_Stamm
Aranon -- ? --- Drogan
Lucian -- ? --- Niptac
```

``` mermaid
erDiagram
  Aranon ||--|| GORN : member
  Drogan ||--|| GORN : member
  Lucian ||--|| GORN : member
  Niptac ||--|| GORN : member
  Argo ||--|| GORN : member
  
```

- [x] Beziehungen fertigstellen  [priority:: medium]