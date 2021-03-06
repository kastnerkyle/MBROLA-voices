LL             AAA         111
LL           AA   AA      1111
LL          AA     AA    11 11
LL         AA       AA      11
LL         AA       AA      11
LL         AAAAAAAAAAA      11
LL         AA       AA      11
LL         AA       AA      11
LLLLLLLLL  AA       AA    111111                       June 05

--------------------------------------------------------------
LA1 - Classical Latin male voice for the MBROLA speech synthesizer

Created by Olivier Bianchi
Laboratory for the Computational Analysis of Speech
University of Lausanne
--------------------------------------------------------------

--------------------------------------------------------------
Table of Contents
--------------------------------------------------------------

1.0 Brief description of the LA1 diphone database
2.0 Files
3.0 Installation and tests
4.0 Announcement
5.0 Acknowledgements

--------------------------------------------------------------
1.0 Brief description of the LA1 diphone database
--------------------------------------------------------------

LA1 is a diphone database for classical Latin, consisting of 
1275 diphones, male voice, and was created in the context of
the author's doctoral project.

LA1 provide diphone for classical Latin pronunciation only
(i.e. 1st century BC).

LA1 uses the SAMPA phonetic alphabet as defined under
http://www.phon.ucl.ac.uk/home/sampa/home.htm. In addition to
the Latin phonemes, some Greek phonemes are included in order
to allow synthesis of Greek words transcripted in Latin caracter.

Long and short vowels are considered different, according to the
newest phonological theories. However, not dinstinction was made
between stressed and unstressed vowels or diphtongs.

Double (geminate) consonants are considerated as the correspondingly
lengthened sound. Double consonants are included in diphone sets
to improve the acoustical database quality.

For further information about phoneme list, see:
Bianchi, O., Orator Romanus. Une synthèse de la parole pour le
latin classique, Université de Lausanne, 2005. (IN PROGRESS)

There are six 'simple' plosives, p b t d k g, and six double
plosives, p: b: t: d: k: g:, and three simple aspirated voiceless
plosives, p_h t_h k_h, and three double aspirated plosives,
p_h: t_h: k_h:, for Greek words transcription:

SAMPA	Graph	Like in

p	p	pater, septem
b	b	bene
t	t	et, terror
d	d	duco, fides
k	c/k	actus, cloaca, kalendae
g	g	flagrum, reges

p:	pp	cuppa
b:	bb	abbreuio
t:	tt	mitto
d:	dd	reddere
k:	cc	assiccare
g:	gg	aggero

p_h	ph	philosophia
t_h	th	Cethegus
k_h	ch	chorus

p_h:	ph	Sapphus
t_h:	th	leget Thyni
k_h:	ch	haec chrysoprys

There are three simple fricatives, f s h, and two double frivatives,
f: s:, and one simple fricative, z, and one double fricative, z:,
for Greek words transcription:

f	f	facile, infra
s	s	soror, filius
h	h-	hoc

z	z-	zema

f:	ff	differo
s:	s/ss	causa/fissus

z:	-z-	zizania

There are three simple nasals, m n N, and two double nasals, m: n:,
two simple liquids, l r, and two double liquids, l: r:, and two
simple semivowels, w j, and one double semivowel, j: :

m	m	amare, manere
n	n	nox, lumen
N	g/n	regnum, relinquo
m:	mm	accommodus
n:	nn	annus

l	l	labor, uel
r	r	gero, ratio

l:	ll	tabella
r:	rr	terra

w	u/v	uoco/voco
j	i/j	iam/jam

j:	i/j	aio/Ajax

There are five short vowels, a E I O U, and one short vowel for 
Greek words transcription, y. Except the central vowel a and the Greek
vowel y, the short vowel appear to have been appreciably more open than the
long:

a	a	caput, amans
E	e	pulcher, epulae
I	i	eximo, ille
O	o	censor, optimus
U	u	amicus, gutta

y	y	cytisus

There is also an 'intermediate vowel' between I et U, 1, that appear only
in particular environments:

1	i/u	optimus/optumus

There are five long vowels, a: e: i: o: u:, and one long vowel for 
Greek words transcription, y:, and three diphtongs, aE aU OE :

a:	a	latrina, ingratia
e:	e	institutiones, uolebam
i:	i	boni, audire
o:	o	impono
u:	u	quamdiu, sternutare

y:	y	Hylaeus, gyrus

aE	ae	rosae, Caesar
aU	au	adauctare, faustus
OE	oe	foedus


--------------------------------------------------------------
2.0 Files
--------------------------------------------------------------

la1.txt    : this file
la1        : the diphone database
test_1.pho : Example : "Multae res ad hoc consilium Gallos
             hortabantur."
test_2.pho : Another example : "Nullum aditum esse ad eos
             mercatoribus."

--------------------------------------------------------------
3.0 Installation and Tests
--------------------------------------------------------------

[part mostly cut&paste from MBROLA help files]

If you have not copied the MBROLA software yet, please consult
the MBROLA project homepage and get it at
http://tcts.fpms.ac.be/synthesis/mbrola.html

Copy la1.zip into the mbrola directory and unzip it : 

   unzip la1.zip (or pkunzip on PC/DOS)
   (don't forget to delete the .zip file when this is done)

Try 

   mbrola la1 test/test_1.pho test_1.wav

to create a sound file for a phrase. In this example the
audio file follows the RIFF Wav format. But depending on the 
extension test.au, test.aif, or test.raw you can obtain
other file formats. Listen to it with your favorite sound editor,
and try the other command files (*.pho) to have a better idea of
the quality of speech you can synthesize with the MBROLA technique.

On Unix systems you can pipe the audio ouput to the sound player as
on a HP : mbrola LA1 test/test_1.pho - | splayer -srate 16000 -l16


--------------------------------------------------------------
4.0 Announcement
--------------------------------------------------------------

This work is only a part of the whole doctoral project, whose goal
is to provide high quality classical Latin speech synthesis, called
Orator Romanus (Laiptts_L). This system, which runs on top of
MBROLA and the LA1 database, included rules for duration
and pitch control. 

For more information contact the author at olivier.bianchi@unil.ch

--------------------------------------------------------------
5.0 Acknowledgments
--------------------------------------------------------------

This database was recorded by Tomas Dubeda, a Czech researcher.
Thank you very much Tomas!

We would like to thank Baris Bozkurt for his efforts in converting
our diphone database to the MBROLA format.

--------------------------------------------------------------

June 9, 2005

Olivier Bianchi

For more information contact: olivier.bianchi@unil.ch
        
--------------------------------------------------------------
