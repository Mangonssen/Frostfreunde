# Beschreibung der Mod 'Frostfreunde'

## Content (English translation)

* Baustab (Building Wand)
  * Blockkern (Block Core)
* Sculk-Hammer (Sculk Hammer)
  * Wächterherz (Warden Heart)
* Antiker Spaten (Ancient Spade)
  * Antiker Schaufelkopf (Ancient Shovel Head)
* Vergiftete Axt (Poisoned Axe)
  * Giftpilz (Toxic Fungus)
* Schwebender Netheritharnisch (Levitating Netherite Chestplate)
  * Shulker-Geschoss (Shulker Bullet)
* Allay-Terminal (Allay Terminal)
  * Allayblut (Allay Blood)
  * Allayrohr (Allay Pipe)
  * Allay-Verbinder (Allay Hub)
* Echo-Bockshorn (Echo Goat Horn)
  * Sculksplitter (Sculk Shard)
  * Echoziege (Echo Goat)
* Leuchtpinsel (Glow Brush)
  * Leuchtessenz (Glow Essence)
* Enderbündel (Ender Bundle)
  * Enderseide (Ender Silk)
  
## Descriptions

### Baustab

    Der Baustab ermöglicht es, maximal 9 gleiche Blöcke auf einmal zu bauen, um eine bestehende Blockformation aus demselben Block fortzuführen. Hierbei ist das nur mit gleichen Blöcken möglich, und diese werden nach Einsatz auch aus dem Inventar des Nutzers gezogen. Sollte der Nutzer beispielsweise nur 4 Blöcke haben, werden auch nur 4 Blöcke platziert (angefangen oben links). Visuell soll eine Art Wireframe als Vorschau gegeben werden.

* Textur: ./textures/building_wand
* Crafting Recipe (Crafting Table Shapeless): Slime Ball + Stick + Block Core

### Sculkhammer

    Der Sculk-Hammer ist grundlegend wie eine Netherite-Spitzhacke, baut jedoch einen 3x3-Bereich ab. Dieser orientiert sich entweder Vertical, sollte die Seite eines Block angeschaut werden, oder horizontal, wenn ein Block von oben, bzw. unten betrachtet wird. Hierbei können nur Blöcke abgebaut werden, die effektiv mit der Spitzhacke abgebaut werden können.

* Textur (animiert): ./textures/sculk_hammer
* Crafting Recipe (Smithing Table): Goldbarren + Netheritspitzhacke + Wächterherz -> Sculkhammer

### Antiker Spaten

    Der Antike Spaten verhält sich analog zum Sculk-Hammer, jedoch ist dieser für alle schaufel-effektiven Items anwendbar. 

* Textur: ./textures/ancient_spade
* Crafting Recipe (Smithing Table): Schleimball + Netheritschaufel + Antiker Schaufelkopf -> Antiker Spaten

### Vergiftete Axt

    Die Vergiftete Axt baut Bäume automatisch ganz ab, wenn der Spieler einen Holzblock von diesem abbaut. Hierbei werden sowohl die Stämme als auch das dazugehörige Laub abgebaut. Die Items werden ganz normal gedropped. Die Axt verliert die Axt proportional zu den abgebauten Blöcken Durability, diese wird aber wie bei jedem Tool von der Unbreaking-Verzauberung affected. Ansonsten sollten sich die Werte wie Schaden und Attack Speed wie bei einer normalen Netherite-Axt verhalten, mit der Besonderheit, dass beim Attackieren ein 3-Sekündiger Vergiftung-1-Effekt applied wird (auf den Angegriffenen). Die Fäll-Mechanik soll ausschließlich bei natürlich generierten Bäumen applien, nicht bei anderen Stämmen / Holz.

* Textur: ./texture/poisoned_axe
* Crafting Recipe (Smithing Table): Moosblock + Netheritaxt + Giftpilz -> Vergiftete Axt
* Probiere gerne, die Visuals mit zur Holzart passenden Partikeln aufzufrischen, aber hier gilt weniger ist mehr (beim Abbauen eines Baums)

### Schwebender Netheritharisch

    Der Schwebende Netheritharnisch ist rüstungstechnisch genau wie die Netherite-Chestplate aufgestellt. Die Besonderheit ist jedoch, dass sie die Elytra-Mechanik auch bereitstellt, ohne, dass eine Elytra equipped sein muss. Außerdem lässt sie den Spieler auf Druck eines bestimmten Hotkeys 7.5 Blöcke in die Luft, also in Y-Richtung schleudern.

* Textur
* Crafting Recipe (Smithing Table): Shulker-Geschoss + Netheritharnisch + Elytra -> Schwebender Netheritharnisch
* Kombinierbar mit Schmiedevorlagen + Verzauberungen sollten sowohl applicable sein, als auch draufbleiben, wenn man den Netheritharnisch upgraded
* Hotkey für Shulker Launch: standardmäßig X; die erfolgreich ausgeführte Aktion spielt den Shulker Schuss Sound, die Aktion hat außerdem einen Cooldown von 30 Sekunden
  
### Allay-Terminal

    Das Allay-Terminal bietet allgemein Zugriff auf direkt nebenliegende Inventare und zeigt deren Inhalt in einem GUI an. In diesem GUI kann man Items aus dem Inventar herausnehmen, sowie hineingeben, solange noch Slots frei sind. Die maximale Stack-Zahl ist hierbei nicht begrenzt, 4 Stacks Erde werden so z.B. als 256 Erde angezeigt. Es gibt zudem ein Suchfeld oben, der als ganz normaler Filter fungiert. Das Terminal ist eine vertikale Slab und betrachtet nur, was an deren abschließender Seite gebaut wird (z.B. eine Truhe). Doppeltruhen werden als ein großes Inventar gezählt.

#### Allay-Verbinder

    Allay-Verbinder können genutzt werden, um mehrere Inventare anzubinden, indem Storage-Blöcke wie Kisten direkt an den Verbinder gebaut werden.

#### Allayrohr

    Allayrohre fungieren nur als Kabel zwischen Terminals und Verbindern. An sie können keine Inventare angeschlossen werden.

* Texturen: ./textures/
  * allay_terminal
  * allay_pipe
  * allay_hub
* Crafting Recipe (Crafting Table von oben links nach unten rechts): Smaragd | Allay-Verbinder | Smaragd | Truhe | Allayblut | Truhe | Smaragd | Glas | Smaragd
* Allay-Rohr: Truhe | Truhe | Truhe | Diamant | Enderauge | Diamant | Truhe | Truhe | Truhe
* Allay-Verbinder: Truhe | Enderauge | Truhe | Enderauge | Diamantblock | Enderauge | Truhe | Enderauge | Truhe

### Echo-Bockshorn

    Das Echo-Bockshorn kann per Rechtsklick gespielt werden, um die Echoziege zu summonen. Es hat einen Cooldown von 30 Sekunden.

#### Echoziege

    Die Echoziege ist eine Ziege mit spezieller Textur. Außerdem ist sie durch den Spieler, der sie beschworen hat, reitbar. Ist die Echoziege beschworen und wird für 30 Sekunden nicht geritten, verschwindet sie wieder.

* Textur: ./textures/echo_goat_horn
* Crafting Recipe (Smithing Table): Echo Shard + Bockshorn jeglicher Art + Sculk-Splitter
* Die Animation sollte der des Wardens ähneln (beim Auftauchen / Verschwinden)

### Leuchtpinsel

    Der Leuchtpinsel konvertiert ausgewählt lichtausstrahlende Blöcke zu Minecrafts minecraft:light-Blöcken. Diese werden direkt platziert und der originale Lichtblock aus dem Inventar des Spielers konsumiert. Der Spieler muss hierfür mit ausgewähltem Lichtblock über den Leuchtpinsel im Inventar hovern und rechtsklicken, um den Leuchtpinsel mit diesem zu befüllen. Die Leuchtkraft des minecraft:light-Blocks hängt von der des konsumierten Blocks ab.

* Textur: ./textures/glow_brush
* Crafting Recipe (Smithing Table): Pilzlicht + Pinsel + Leuchtessenz -> Leuchtpinsel

### Enderbündel

    Das Enderbündel erlaubt dem Spieler ganz einfach Remote Access auf die persönliche Enderchest.

* Textur: ./textures/ender_bundle
* Crafting Recipe (Smithing Table): Enderkiste + Bündel + Enderseide -> Enderbündel