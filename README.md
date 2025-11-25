
1. Diferențele dintre iluminarea reală și iluminarea din OpenGL

Iluminarea reala:
- Lumina se propagă fizic (reflexii, refracfii, umbre naturale).
- Interactiunea luminii cu mediul este complexa si continua.

Iluminarea în OpenGL:
- Este doar o aproximare matematica.
- Nu există umbre reale, reflexii sau refractii automate.
- Lumina afecteaza doar obiectele vizibile direct, fara propagare.

2. Numarul de surse de lumina suportate in OpenGL prin OpenTK

- OpenGL in modul fixed-function suporta maximum 8 surse de lumina: GL_LIGHT0 … GL_LIGHT7

3. Definiți iluminarea de material și specificați unde și când este
utilizată aceasta.

- Iluminarea de material reprezintă modul în care un obiect reflectă lumina, prin componente precum:
  - ambient – culoarea în lumină difuza
  - diffuse – culoarea sub lumină directa
  - specular – reflexii de tip lucios
  - shininess – concentratia reflexiilor
- Este folosită în definirea obiectelor 3D pentru a calcula iluminarea cu modelul Phong.

4. Care este efectul asupra diverselor obiecte la activarea unei surse de
lumină secundare (per pct. 3), comparativ cu utilizarea unei singure
surse de lumină?

- Obiectele devin mai bine luminate si mai detaliate.
- Apar reflexii suplimentare din directii diferite.
- Iluminarea devine mai uniforma si mai realista.
- Zonele foarte intunecate sunt reduse.

Observatii:
- Cu o singură lumina: zone puternic luminate + zone întunecate.
- Cu doua lumini: iluminare mai echilibrata si mai realista.
