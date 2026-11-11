# Photographs to shoot

Every photograph on the site today is a vetted library frame of **another** café, used as a
stand-in under the licences on `credits.html`. Nothing on the pages says so, and nothing should:
they are placeholders for the client's own pictures, and the site reads as finished with them.
Replace them before launch.

**How to shoot them:** half a day with a local photographer, or one morning on a phone.
1× lens, window light, no flash, no filter. Shoot both landscape and portrait of each subject.
Hands and backs only — no recognisable faces, no other business's branding in frame.

| Where it is used | File on the page | What to shoot instead | Crop |
| --- | --- | --- | --- |
| Home hero | `photo-m61716670` | The room from the door, or the shopfront straight on, in daylight | 3:2 landscape, calm on the left |
| Home, Find us | `photo-m61713103` | The counter with the machine, straight on | 4:3 |
| Home, Popular today | `photo-m201752739` | A drink being made at the bar, hands only | 4:5 portrait |
| Home, Popular today | `photo-m61714648` | Breakfast on a table in the window | 4:5 portrait |
| Home, Inside the café (wall of six) | `photo-m187311853`, `photo-m28989985`, `photo-m61713028`, `photo-m61713362`, `photo-m62054123`, `photo-m189498721` | Six details of the room and the counter: the pastry case, a laid table, the window seat, a cup going out, the courtyard, the bar from the end | 4:3, one light and one grade across all six |
| Home close | `photo-c141` | A finished drink on the counter | 1:1 |
| About hero | `photo-m147143963` | The room early, before service | 3:2 landscape |
| About, the story | `photo-m147143894` | The people who run it at work, from behind or hands only | 1:1 |
| About, what we believe (strip of four) | `photo-m61712989`, `photo-m147143898`, `photo-m62054123`, `photo-m61713362` | Four details: the grinder, a tray out of the oven, the day's board, the till corner | 1:1, one light |
| About close | `photo-m189498721` | A full room at mid-morning | 1:1 |
| Menu hero | `photo-m61713028` | The counter with the day's food in it | 3:2 landscape |
| Menu, breakfast and lunch | `photo-m187311853`, `photo-m28989985` | Two plates as they are served | 4:5 portrait |
| Menu, drinks and desserts (strip of four) | `photo-m201752739`, `photo-m61714648`, `photo-m147143894`, `photo-m147143898` | Four drinks and cakes on one surface | 1:1, one backdrop |
| Menu close | `photo-m61713103` | The counter from a customer's height | 1:1 |
| Contact hero | `photo-m189498721` | The front door from the pavement | 3:2 landscape |
| Contact, Find us | `photo-m147143963` | The shopfront straight on, with the sign readable | 4:3 |
| Contact, Send a message | `photo-m28989985` | The room from the counter | 4:3 |
| Contact close | `photo-m61712989` | A coffee being handed over | 1:1 |

**Replacing one:** drop the new file into `assets/img/`, then change the `src`, `srcset`,
`sizes`, `width`, `height` and `alt` on that `<img>`. Set `data-source="client"` in place of
`data-source="library-057"`. When every library frame is gone, delete the credits line and
`credits.html` from the footers.

The site also has no photograph of **tables, the terrace or pastry** — the library holds none
of those for a café, so those slots were filled with other subjects. They are the first
pictures worth shooting.
