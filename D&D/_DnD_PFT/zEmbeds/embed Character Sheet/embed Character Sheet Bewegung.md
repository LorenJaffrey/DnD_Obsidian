|                            |                                                               |
| -------------------------- | ------------------------------------------------------------- |
| Gehen                      | `=this.Bewegung*1.5` m (`=this.Bewegung` Kästchen)            |
| [[Spurt]]                  | `=this.Bewegung*3` m (`=this.Bewegung*2` Kästchen)            |
| [[Hochsprung]] mit Anlauf  | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)` m   |
| [[Hochsprung]] ohne Anlauf | `=round((floor(((this.Attribute.Stärke)-10)/2)+3)*0.3,2)/2` m |
| [[Weitsprung]] mit Anlauf  | `=round((this.Attribute.Stärke*0.3),2)` m                     |
| [[Weitsprung]] ohne Anlauf | `=round((this.Attribute.Stärke*0.3)/2,2)` m                   |