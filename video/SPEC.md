# SPEC — «Un dilluns de setembre» (versió comercial)

GOAL:    La coordinació de LANAU112 acaba el vídeo pensant «ho vull»: tot el centre (alumnes, cicles,
         mòduls, pràctiques, pagaments, professorat) en una sola base de dades ben organitzada,
         gestionada des d'una web.
OUTPUT:  HyperFrames, 1920 x 1080, 30 fps. Idioma: català.
TIME:    50 s x 30 = 1500 frames. Sense música (no hi ha font de música en aquest entorn); efectes
         de so a cada acció visible.

FETS (de lanau112.cat via cerca): LANAU112, Sabadell (Pg. Can Feu 17-23). Centre d'ensenyament
         en seguretat, emergències i salut. Cicles: CFGM Emergències Sanitàries, CFGM Cures
         Auxiliars d'Infermeria, CFGM Emergències i Protecció Civil (presencial i semipresencial,
         2.000 h, 2 cursos), CFGS Coordinació d'Emergències i Protecció Civil.
         Noms d'alumnes, professors, empreses i xifres: IL·LUSTRATIUS, marcats «Dades d'exemple».

LOOK:    ground #F4F6FA, ink #101A33, line #D8DDE6;
         brand #4E70B0 (blau corporatiu de lanau112.cat), logo #3F3F3E + #4E70B0,
         ok #17985A, warn #E89B0C — només per a estats (pendent / resolt).
         L'accent brand surt: la paraula clau de cada títol, el botó d'acció, el tauler i el final.
         Display: Montserrat 800, 96 px (8.9% alçada), tracking -3%. Títols secundaris Inter 700 56 px.
         UI: Inter 400/700, mínim 26 px després de l'apropament.
         Medi: la pròpia UI de la plataforma i les cel·les d'un full de càlcul; ombres 0 12px 32px
         rgba(18,32,47,.12); radi 14 px; sense gra, sense vinyeta.
OBJECTS: full de càlcul (graella, capçalera de columnes A-F, cel·les en vermell/groc), post-its
         groc #FFE27A girats ±4°, targetes de taula de BBDD (capçalera color + camps amb icona de
         clau), finestra de l'app (barra lateral blanca, taula d'alumnes, xips d'estat), cursor
         negre 64 px, horari setmanal, tauler amb barres i anell.
MOTION:  entrada expo.out 0.6 s; moviment power3.inOut 0.5 s; càmera power2.inOut 0.8 s;
         sortida power3.in 0.3 s; xips amb back.out(1.6); stagger files 0.05 s, paraules 0.08 s.
SHOTS:
  1  0-6 s    intro      Full de càlcul ple de vermell + post-its; preguntes grans una a una.
                         So: typing, pop als post-its. Sortida: les cel·les s'enlairen.
  2  6-13 s   bbdd       Les cel·les aterren en 6 taules connectades (Alumnes al centre); les línies
                         de relació es dibuixen. «Una sola base de dades». La taula Alumnes creix
                         i es converteix en la finestra de l'app.
  3  13-31 s  alumnes    App: cicles reals a les pestanyes, llista amb estats; clic a filtre
                         «Sense pràctiques»; clic a l'alumne → fitxa; assigna pràctiques (xip
                         verd), envia recordatori de pagament (toast). Clics i pops.
  4  31-37 s  professorat Horari setmanal es reomple amb mòduls; càrrega d'hores per docent.
  5  37-44 s  tauler     Tauler amb xifres d'exemple; riser → impacte a 38.6 s.
  6  44-50 s  tancament  Inundació de color brand; frase final; marca LANAU112 + crida a l'acció.
BANNED:  fons fosc buit; brillantors, partícules, gradients lila/blau, vidre; tot centrat;
         tot apareixent amb fade + slide-up; tres targetes en fila; logo petit en una cantonada;
         títols que es mouen mentre es llegeixen; xifres inventades sense etiqueta d'exemple.
QA:      2.5 s (preguntes), 9 s (esquema complet), 16 s (filtre), 25 s (xip verd), 34 s (horari),
         41 s (tauler), 48.5 s (marca + CTA).
