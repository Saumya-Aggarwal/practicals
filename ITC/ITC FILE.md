# ITC FILE Transcript

Source: OCR transcription of the handwritten/photo PDF stored as ITC/ITC FILE.pdf.


## Page 1
```text
EXP DATE EXPERIMENTNAME MARKS TOTAL SIGN.
HaniduBod 1+man loclin
96/2/26 Write a Scilab pog+implement
shanon Funo
16/2126 pousidu!o mo bord write a scilab
lempel ziv enco@ty
23/2126 Toculculede enoby cundHutual injo
yNoisy and Noisles
23/2/26 and MI Rdaduo docr6
Jree and gsc
16/3/26 dorencociry Toimplenent the ago and
dleccdiryy yel'e code.
23/3／K mnpoixap mobr decocliu Linear Toimplement the Blouk Code 3013
30/2/26 YHanonuohyonineop To imblement algorithm
614/26 convolutaHon code by
Toimplenen+ Hhe codeTrellis
13/0124 hpoua rode. ollwdiy
```

## Page 2
```text
EXPERIMENT-1
AM:- gencration Write and Scilab ewaluation uoxboxd 0implement and cooliny Mlyman codiry agorithn yieingy and decocliy
lompute entropy; avg.linh
Throg: a romprcssion Heygman set hapu!adstI-uytuobn cocling sovzte a botom-up ,varioble -lengh,lossless symbols using codeword a binary objechive lengthis minimized istorepresent aphabetn
This nmos achievec wuay Hhat mhoox can be avg nibaid u:bdp property which any other elictatus
Rndxdsiupompo) Hhar no lsd vitol dor unabigours deco-
ding, without 计. constructiry tu/dmdn tree
aprobability Thts nmap-dat Leaves inormation ，Hhe he based procesc cllqorithm methods Hhe Hhe continues symbols yuncthons 4.0 probabitiu 00 Helyman wih unHLa he Jorm(d. starhswit ymbol algori Hhm Hhenaast sing le mouiny Lowutprobablitie Hhe “weahest" root pode with olcurrene.Unlike ensure from Hhat te
the most Jreguent Symbols
Hhe oot resuitiny
Wigher dregvency data.
```

## Page 3
```text
#fource → symbols ，5，S2,3，S4，55}
Probabilites 0.25, 0.3, 0.15 , 0.05 , 0.1, 0.15]
0.30—-->0·30 →0.40 8.60
5。 0.25----——>0.25. 0·30 0·30 oh.o
S2 0.15- 0.15. *0.25 0.4 0.6
55 0.15 0.15 0.3
Sy 0.10 0 0.15 0.15
53 0.05
1.00 Entropy =H=-P)log(ni)
=0·5+0.52+0·41+0.22+0·33+0.41 —0.15l0g0.15
2.39bits/s00rce
Symboe 50 (odeword 10 Length 2
S1 01
S2 000 3
53 3
54 110 33
S5 001
Lavg =0.25x2+03x2+0.15x3+0.0513+013+0.15x3
=0.5+0.6+0.45+0.15+0.3+0.45
DoquBs/s+!9gh·=
ecieny=n= Lmin Lavg Lavy H 2.45 2.39 0.975
)=97.5
```

## Page 4
```text
X
1 2 clear; clc;
symbo1s=["s0","s1","s2","s3","s4","s5"]; [0.25.0.300.150.050.100.15];
6 0=
9 8 for·i=.l:size(p,"") H=H-p（i)*1og(p(1))/1og(2）;
11 10 disp("Entropy-H.=."+string(H)+".bits/source"); end
12 13
14 16 15 L size(codes,l); .zercs(n,l);
17 18 for i=l:n L(i)=.length(part(codes(i),1:c));
19 20 end
21 22 23 for i=l:n Lavg =.0; Lavg =Lavg.+ p（i）*L(i）;
24 25 end
28eta =H / Lavg; 27
29 30
32 31 33 34 disp("Symbol.....Frob.....Codeword.....Length"): for i=l:n disp("."); mprintf("is. syzbols(i),p(1),codes(1),L(1)); 21 d\n",
36 35 end
37
```

## Page 5
```text
OUTPUT:
Scllab 20260.1Console "Entropy H -2.3904686 bits/source"
"Average Length = 2.45 bits/symbol"
"Efficiency=97.570146"
so "Syrabol 0.25 Prob 10 Codeword 2 Length"
S2 S3 S1 0.15 0.30 0.05 01 000 111 2 3 3
S5 S4 0.15 0.10 110 001 3 3
```

## Page 6
```text
EXPERIMENT-2
#AM:Writt generation ancd evauluation at shannon sono coding and
boinohdoxuo2nduBurpop unaPbBupopuobu
Ry# Shannon -Fanu coding a top-down,variable eLcngth
soUrce coding tech nque designed
IHs primary symbols using binary alphabet insuch a kpm
the querage codeword length is mlnimizcd. This is achievec
Hhrough preJinproperty which clicta+us HhatnoCodew
po can be cioxd any loclecord.This pro
Rtr>d is vitae unambigous without it ，a
bitstream Lihe oll1'could be interpreted a muitiple
diyerent symboe combinatiorg ,rendering the communicatian
inccherent.
The cllgorithms dunchion Hulyman tree base
onHhe probcab lities gsymboe occuryence .Unline top-down
methods tyyman sturkcuith He"wcahust ir/ormation
Hnesgmbols wsith he Lowest probabilities. These aYc
p24 leol nodes ond qrc repeadtedly paired and
merqed into intexncel nocley whase value is the sum
single childrenls root node probabieitics.Thisprocess a probability rontinucsunt' puxo/'.s!
moving Jrom Hhe leaues +o Hhe rcots ， Hhe algorithm
ensures ++ most drequentsymbols
```

## Page 7
```text
Source
eymbolu:0，1#，3，5u5}
Probalitiu : 0.25 , 0.3 , 0.15, 0.05, 0.10, 0.153
0.30
0.25 O
0.15 O TIT
$5 0.15 O 一
h5 0.16 一
53 0.25
Symbol CODEwoR) 10 LENGTH 2
50 'S GO 2
S2 100 3
53 3
Sy 110 3
55 3
HP(ni)LogP(xi)
0.25 - 2(0.15 l0g 0.15) - 0.1 log2a1 -0.0510g,005
a.39bits1 source =(03x2)+(0.2sx2)+（0.15×x2)+C0.15x3)(01x4)+
bm0《#丽 =06+0.5t0.3+0.45+0.4+0·2 (0.65x4)
= quc/ sh·
(H==Bu1 L =2.39 2.45 0.975=97.51.
```

## Page 8
```text
CODE:
TTC2.sdx
2 1 clc; clear:
6 S p=[0.25.0.300.150.050.10.0.15];
8 for.1=1:size(p,"") H=.0;
10 9 end B=B.-p(1)*1og(p(1))/1og(2）;
1 disp("Entropy·H.-."+string(H)+"-bits/source");
n.=.size(codes,1); L.=-zeros(n,l):
at 17 for.i=l:n
19 20 end L(i)=.length(part(codes(i),l:)y;
21 22 Lavg.=.0;
23 24 for-i-l:n Lavg = Lavg·+·p(i) *L(i）;
25 end
27 28 eta-=B-/Lavg;
30 29
31 32 disp("Symbol.....Prob.....Codeword.....Length") disp("-");
33 34 for-i=l:n
35 36 mprintf("ts.. symbols(i),p(i),codes(i),L(i)); t.2f din
38 37 end
Line30,Column0.
```

## Page 9
```text
OUTPUT:
sellab20260console
"Average Length = 2.45 bits/symbol" "Entropy H -2.3904686 bits/source"
"Efficiency-97.570146"
so "Symbol 0.25 Prob 01 Codeword 2 Length"
S2 S1 0.30 0.15 100 00 2 3
S3 S4 0.05 0.10 111 110 3 3
ss 0.15 101 3
```

## Page 10
```text
EXPERIMENT-3
#Am: Towrite a Sailab progrom to implement the algorihm
dor genexation and cwaluation the Lempel-Ziv clichionaxy
method ond tu compute Entroby， Avyg Code Lurgth Cpo puD
eljecieney bosnudunbB
R# Data compression isan important concept pun uu
Coding (1T) . I+ reducex the number bitsrequircd repres
ent datawhile nlormation
6sion tchniquesare broaculy classigico into Rsso7 ssor pun
less agorithm Rrpimos!
used losselcss comperssion technique.
The Lempel -Ziv algorithm worhi dy nomically building
ux24Fodβ .mm scanning theinput data.Tnstead
asigning Jized codes
sequences
new sequences
hxou data containing repcated battems.
The mcin idee s：
>Reac Hheinpot scquence rom lyttorght
-)Maintain a dichionary previously seen p atterns.
->Add m4 petem
-)Usc dictionary indice toreprescnt data eicety
```

## Page 11
```text
#Example
Numerical PosiHon Dictonary LocaHon Subsequenle Numerical RepresentaHur Binary pompo7
0001 2 00001
2 0010 00100
3 001 3 60110
0100
6 5 0110 0101 31 2
7 0 5 01010
8 01000 CG 5 2 61611
L 1001 2 2 00101
10 1010 9 1 10010
> Total No. bits = 20
= No. 0's = 13
=（1)d 20 =0.35 P(0)=130-65 20
hdauu # H=-<p;log.
d2
Substitute values
=> H= - [0.6s e0g(0.6s) + 0.35 l0g(0.35]]
H = - [-6.403 — 0.5301]
H=0.98406bits/s0uce
```

## Page 12
```text
5bits
Total phrcsts=10.
Formula-> Lawg ELi n
Lavg Sbitstsourke3.32bits/source
Bun!3 (= Sutaitte 0.98406
B.32
降K9.661 ·29.66
```

## Page 13
```text
*tic.sd X
clear; clc:
n= length(msg): msg="101000010100000111110";
9 8 disp(msg); dict index =.0; dictionary =[]:
11 10 i=1;
13 12 while.i<=n
14 15 current = part(msg,i）;
17 16 j=i;
19 while-#T
20 21 found.=.0;
for.k.=.l:dict index if dictionary(k) current-then
1 2 23 2 25 2 22 2 2 end found.=1; break;
end
30 if.found =-1.-j<.n.then j=-j.+.1;
32 31 else current =·part(msg,i:j);
33 34 end break;
35 36 end
37 38 dict_index.=.dict_index.+.1;
39 40 dictionary(dict_index)= current;
41 42 i.=.j.+.1;
43 44 end
45 46 disp("."); disp("Generated-Lenpel-Ziv.Dictionary:");
48 47 for-i=.l:dict_index
49 50 end mprintf("td..-->..ts\n",i, dictionary(i));
51
```

## Page 14
```text
51 countl=.0;
2345 counto.=.0;
56 55 for-i=.l:n if·part (msg,i) =="1".then
58 57 -else countl =countl +-1;
59 60 .-end counto.=.counto.+-1;
62 61 end
63 64 po=.count0./n; pl.=.countl./.n;
65 66 H=.-（p0*1oq2(p0).+ p1*1og2（p1)）;
67 68 disp("-");
69 70 disp("Entropy-Calculation:");
71 72 mprintf("Total-Bits.=.&d\n",n); nprintf("No.-of-ls.=.&d\n",countl);
73 74 mprintf("No.-of-Os-=.d\n",counto); mprintf("P(1)=..4f\n",pl);
75 76 mprintf（"P（0).=.4f\n",p0); mprintf("Entropy·(H)=.&.4f.bits/source\n
77 78 avg_length =.1og2(dict_index);
79 80 disp("-");
81 82 mprintf("Dictionary-Size=.d\n",dict_index); mprintf("Average.Code.Length-=-.4f-bits\n",avg_length);
83 84 efficiency =.(H-/avg_length)* 100;
85 86 nprintf("Coding-Efficiency-=..2f·\n",efficiency);
87
```

## Page 15
```text
8 7 > 011 000
10 6 > 11 10
Total Bits = 21 "Entropy Calculation:"
No.of 0s= 12 No.of1s=9
P(1)=0.4286 P(0) =0.5714
Entropy (H) = 0.9852 bits/soyrce
Dictionary Size = 10 Average Code Length 3.3219 bits
Coding Efficiency= 29.66号
```

## Page 16
```text
EXPERIMENT-Y
WW# 下o calculatt entropy and Mutual inormation
Noise-grce and Noisy channel.
: h204L #
In acommunicator sys+em, a sourze produces sym bals wite
certain probabilities.
a discrete SouTeprodlucex symbols ui, x2.. xn wit
probabilitic P(u) ,P(xz)...P(un) +hecntropy mcasues the
average ingormation per symbol.
Bdouu3 :m pubap!
hug oxop sobrce:-
Rdoyun is deyined cu:-
H(x,y) =-<≤pCx,y)∞gP(x,4)
Mutual iryormation guen by -
=H(x) H(x14) LP(X)P(y)
(x1) +1-(H1
=x
I(x;4)=H(x)
Mutual ingormatibn ismaximum.
Now, ina noisy chonnel Lihe , Binary (s ruumm apuuks
P:- noise 1-p-signal
```

## Page 17
```text
As，pin（rcass mutal gormaton noise decreases channel increau ond nenle the
an source
Po=0.5 and 0,=0.5
wehaved 42 channel ncise-gree (Bsc) wih channee P=O.1. wahs haoug # puo
Laculating Entropy:
=（x)H —（0.5 10g(0.5)+0.50g2（05）)
l∞q（0.5)=-1 d2
H(x)=-(0·5(-1)+05（-))
H)=1
(ase-liNoise-geee channel:
y=x
0.5 and P=0.5
Henle; H（4)=1
Joint probability P（x,9):
P(x,4)
O 0.5
D
0.5
```

## Page 18
```text
##aculating Joint Entropy H(X,9):
H(x,4）=-p（x,y)0g2(xy)
[0) 9·0(bs]=
H（x,y）=1
#Nowcalculchion mutual inlormation:
=（：x)I H(x)+H(y)-H(x,y)
1+1-1
1
Case-I-Noisy Channee 0.1
n=0 6= 0.9 Y=1 0.1
n=1 0.1 0.9
Joint probabilites:
p(x,4)=p(x)P(y/x)
P(n)=U.5
(9'0) d 0·5×0.9=0.45
P(0;) 二 0·5x0.)=0.65
p (1, 0) 三 0.5x0·1 二0.05 Sh·0
p（11)=0.5x0.9
P(y=0)=6·45+0.05= 0.5
P(Y=1)=0.06+0.45=0.5
0,H(y)=1
```

## Page 19
```text
# joint entropy=
[（0.45 Q0g（0.45)+2（0.05 log,0.05) 2
H（X，4)=-[2(0.45x-1.152)+2[0.05x-4.322)]
H(x)=1.469
#MutualIngormation:-
I(x;y)=H(x)+H()—H(x4)
I(x:4)= 1+1
0.531
```

## Page 20
```text
entropy_cakc.sdx
1 2 clc: clear:
3 1 function H - sntropy calc(p)
for i=l:length(p) 日=0:
if p(i) > 0 then H =H.-p(1)*1og2(p(1));
end
7 end
12 disp("- endfunction -NOISEFREE-CHAMNEL
13 14 Px=[0.50.5];
15 Hx=ntropy calc(Px）:|
17 16 Hy -entropy calc(Py):
18
19|Pxy= diag(Px）;
20
21Exy-0;
22 for-1-1:2
for-j=1:2
1f·Pxy(1,j)>0.then
222527 Bxy=Hxy-Pxy(1,J)1oa2(Pxy(1,j）):
end
28 end end
29
30 XHH+·xH=XI
32 disp(Joint EntropyH(x,Y).#"+ string(Bxy)); disp("Entropy-H(x) +atring(Hx));
33 disp(MutualIntoxmation-I(X:Y).="+string(Ixy));
34
```

## Page 21
```text
S4 53 diSP("----.NOISY CHANNEL.-
SE 55 p=0.1:
57 58
59 60 Pxy_no1ay#.2er09(2,2):
62 E1 for i-l:2 for·j=1:2
E3 E4 end Pxy_noisy(i,j)= Px(i)'P_y_given x(i,j）;
E5 end
EE 67 Py_noisy = sum(Pxy_noisy,
68 E9 Ex=entropy calc（Px）;
71 70 Ey_noisy = entropy calcyPy_noisy);
72 73 fori=1:2 Exy_noisy=.O;
74 75 for j=1:2 if Pxy_noisy(i,j)>O then
76 77 end Hxy _noisy= Hxy_noisy - Pxy_noisy（i,j)*loa2(Pxy_noisy(i,j）):
78 79 end end
80 el Ixy _noisy = Hx + Hy _noisy - Hxy_noiay:
e2 83
esdisp("Jcint Entrory H(x,Y)="+ string(Hxy_noiay)) 84 (（ketouAg）uz=x）H doau)de
```

## Page 22
```text
Output:
Schab 2026.0.1 Console
"Entropy H(x) -1" NOISE FREE CHANNEL
"Joint Entropy H(x,Y) -1" =1
NOISY CHANNEL
"Entropy H(x)- 1" "Entropy H(Y) = 1"
"Joint Entropy H(x,Y) 1.4689956"
"Mutual Information I(X;Y) = 0.53l0044"
```

## Page 23
```text
EXPERMENT-5
#AM:WriteaMATLA program to comuteenhropy and
mutuali
channee.
#Tcory:Injormation Thcoy, cnropy measures the cncertuinity
ingormation conten t a souvte,whilc mutucl injormatioa
measureHheamount
ond octput d a channel.
Entropy CH):-
Fer a dliscrete souyce with probabilitics P(ni:
H(x)=-Epni)eogHni)
Mutae InyomationI):
Mutual iglormaon behueen input X and ootput Yis given by:
I(x:y)=H（x)-H(x1y)
where:
>H(x) = entropy orinput
·>H(xIy)=conditionalcntropy
ERRoR Free Channel:
Jn an erro- Jree channel , the output is cnactly he samea
P(41x)=1
60, (H（x19)=O
I(x;y)=H(x)
c)This mcansmanimum inyomation Iis tronsmited with no less .
```

## Page 24
```text
#Examp1e
P(0) = 0.5 P(1)=6.5, Fo 5 = =0·1
Entropy.H(x):
H(x)=gb)
H(x) = - 0.5 eog0.5 + 6.5 log26.5] 02
H(x) = - [0.5(-1) + 0.5(-1)] = 1bit
Error -Free Chonnel:
For an error yree channcl:
H(x1]=
I（x:y)=H（xH（x14)
I(xiy) -0=ibit.
3)Binary Symmchic Cnannel:
b=6·L
(ondiond ntong →H(14) =-plog2b -(1-g(1-b)
— o.1 Log. 0.1 + 0.9 log0.9]
= —[0.1x(8:32) + 09 (-0.152)]
=) 0.332—0·137)
=) 0.46abit
Muhual informat'on
I(x;)=H()—H(/x)
26.531bits 69h·0-1=
```

## Page 25
```text
CODE:
"ITCExp.sax
1 clc;
2 clear;
3 11-EXP.5
4 p0=.0.5;
5 p1.=.0.5;
6 p.=-0.1;
8 Hx.=.-(p0*1og(p0)/1og(2)-+·p1*1og(p1)/1og(2));
9 disp("Entropy·H(x)·=".+-string(Hx)·+."bits");
10 11 HxY errorfree.=.0;
12 I errorfree =-Hx - HxY errorfree;
13 14 disp("-");
15 16 sdisp("H(x|Y)=."+string(HxY_errorfree)); disp("Error-Eree.ChanneL:");
17 7disp("I(x;Y)-=.".+ string(I_errorfree)-+"bits");
18 //.Conditional entropy·H(xly)
19|HxY.=.-(p*1og(p)/1og(2)+.(1-p)*1og(1-p)/1og(2));
20 21 disp(".");
22 disp("Binary.Symmetric.Channel:");
23disp("H(x|Y)=."+·string(Hxy)-+.".bits");
24 2s//-Mutual.Information
26I=HX-HXY;
27 28disp("I(x;Y).=."+·string(I)+"-bits");
29
Line 7,Column 0.
```

## Page 26
```text
OUTPUT:
Scllab 2026.0.1Cons0l
"Entropy H(x) =l bits"
"Error-Free Channel:"
"H(X/Y)=O″
"I(x;Y) =l bits"
"Binary Symmetric Channel:"
"H(X/Y) =0.4689956 bits
"I(X;Y) =0.5310044 bits"
```

## Page 27
```text
EXPERIMENT-6
#AM: Write a MATLAB program to implement the algorihm
Jorencocling and dlecocdng Lincar Bloch Code.
and error
correching tades inwhicheach codcwordis generadted Jrom a
number input bits. An (n,k) lincar blocl code mups 1
message bit inho n-bit codle cusords , where n>k.
The encoding pergormed using a GrcneredorMatrin(Gn):
C=m.
where=> )m=
(=cocleword（1xn) generato matrin(Kxn)
#Decoling Drocess
Atthe reciever, the recieved vector r is cheched osing Hhe
(H)()
S=Y.HT
where:
7] s=0 , no cxror is deected >sO, an error prescnt and
）odpuo+(= (dmin errors
:qd(=
dmin-1 2
```

## Page 28
```text
#Enample:
Griven) G= 0一一0 bosu xo peormo pu 011
00101 2) Decocle recieved scquence lo161
n=6,K=3,q=3
[：]U []=[m][P]
[cc2(3]=[m,m2m]
=mm
C2=m田m田m
C3=mm3
[110] m=0 m2=
C=1
oclecoxd=m
302 jollal =h Par Chcekmatriu!
S= 4HT [PT:T]
S=[1011][ O
O O []=>
11
O 0１ E=000001]
```

## Page 29
```text
E=[000001] y=[101101]
loectedCodeworcl=E
[01101]④[00000]
[161100]
```

## Page 30
```text
CODE:
*TTCEXp.sa X
clc:
clear;
12345 G=.[1-0.0.1-1.1; //.EXP.6
0-1-0-1-1-0;
6 00-1-0-1-11
7 m-=-[0.1-1];
8 c=-modu1o（m.*-G,92);
9 disp("Message:");
10 disp(m);
11 disp("Encoded.Codeword:");
12 disp(c);
13 Y=-[1-0-11.0-1];
14
15 disp（".");
16 disp("Received.Vector:");
17 disp(y);
18
19 P [11-1;
20 1-1-0;
21 0.111
22
23H.=.[P'eye(3,3)]; 24
Line 10.Column8. 25ldisp".
```

## Page 31
```text
TTC Exp.sdx
22
23H=[P′.eye(3,3)];
24
25|disp(".");
26disp("Parity-Check Matrix H:");
27disp(H);
28s=·modulo(y *H',2);
29
30disp(".");
310 disp("Syndrome S:");
32disp(S);
33if S==.[00 0]-then
34 disp("No-Error");
35 e=·zeros(1,6);
36lelse
37 disp("ErrorDetected");
38 e=[0-00001];
39end
40disp("Error·Vector:);
41 disp(e);
42corrected = moulo(y +·e,·2);
43c disp(".");
44|disp("Corrected.Codeword:");
45|disp(corrected);
46
```

## Page 32
```text
OUTPUT:
"Hessage:" 0. 1. 1.
"Encoded Codeword:" 0 1. 1. 1. 0.
"Received Vector:" 1. o. 1 0
"Parity Check Matrix 1. 1 1. 1. 0. 0. 1. 1. .0 1. 0. H:" 0. 1. 0. 0.
"Syndrome 0. 0. S:" 1.
"Error Vector:" "Error Detected"
0. 0. 0. 0 0. 1
"Corrected Codeword:" 1. 0. 1. 1.
```

## Page 33
```text
EXPERIMENT-7
encocding Bbupoap puo biocar
:RO#
Cycliccodesarespecial caseclass y Untar bloch cocesm which
These codu are wicdely used doue totheiy omy #ompopmon#you decient hardwsare
implementaticn.
Encoding Process:
>Themcssage is representtcd as ce polynomial m (n)
Then clivicled (mbrououhod xaponinbytha
((a)=m（a).nnR+R（n)
Where: R(o) =remeinder s
Decocliy Arocess:
>Thereceivel polynomalr(x) & diviced by g(cm) :
#ru) modgée)
remainder=O→no crror
9puu
I+s widey used in CRl( (yolic Redonday chch)
```

## Page 34
```text
#Enomple:
Grenerate [++en=(mol)7uouhjod 1n(t)
0 n=7,K=4， q=3
#>Encoding
u n²+1=μ（n
ituren en+sn nu(e)=nμ(∞)
++
²—Rem
(()=n2
22 codevector
c= 100 X： 二 M:C 101:100
Now or decocliny pom!9-
0011019 (n)+s+=
1+v ++
Bemainder =0 = No err6
μ=6101
```

## Page 35
```text
CODE:
7th cydic code.sci
1 clc: clean:
3 4 n
S E K n 4：
7 01011
10 9
11 12 disp(m9g)
14 13 6 [10.11]
15 1E dividend =-temp; tenp =-(nsgceros（1,r)]：
17 18 f0二1=1:k
19 20 ifdividend（i).==.1.tnon forj-=.1:1ength(g)
21 22 end dividend(i+j-1)=xor(dividend（i+j-l),g(j)):
24 23 ena end
25 26 zem.= dividend(k+l:n）:
27 28 disD（"Paricy.Bica:"）：
29 30 disp（rem);
31 32 codeword=msgrem]:
33 34 disp"Enccded.codeuord:"): diap(codeword)
3S 36 recy= codeword:
37 38
39 40 disp(recv):
41 dividend2.= recv;
```

## Page 36
```text
40 41 dividend2=recv:
421 43 fori=1:k
44 ifdividend2（i)==Ithen
45 forj=l:length（g)
46 dividend2(i+j-l)= xor(dividend2(i+j-l),g(j));
47 end
48 end
49 end
50
51 syndrome = dividend2(k+l:n):
52
53 disp("Remainder-After.Decoglng:
54 disp(syndrome):
55
5E if-sum(syndrone)== then
57 disp("uo-Error"
58 else
59 60 end disp("Error.Detected"):
T3
E2 decoded=recv(l:k):
63
E4 disp("Decoded-Nessage:");
E5 disp(decoded);
6el
```

## Page 37
```text
OUTPUT:
Sciab2026.0.1Consoe X
line 0. 1. 21 of executed file D:\iTc\7th cyclic code.sc1 0.
Jndefined variable:xor
```

## Page 38
```text
EXPERIMENT-8
b4bwboP Convolutatonalcocle Code Tree.
#Theory: Convolutonal code are type BuHo-o? coclas
6i+ Hheoutput oupnhp inputbits. only o These cocles are cuidely current inbut
used 1n lommunitation Sy stems dor reliable data transmission.
Aconv olut'onal encodercon&ists
Shyt register modulo-2acldtrs Gcncrator segpence
The cncoder processes input hits sequentally ond producu outout bifs
based 6n rCdundancy
detechion and correction.
Acode Tree is a graphicalreprescntation encodiwy proccss
>Each nocc represcnkastat the encoder
·)Branches "( ) !ndu
shod(. > Each bronch is labtled with he tcorrespondiry drem root + nodu ebresent pponun sequenLes. output bit.
Encocling Process :
+!9 odu! o
hs< Hhebitintothe registes.
Compute AppendouHputbih outputs buisn into the enroded sequence. gencratoy polynomicls
#Cocc Rate 长 K=no. inpet bis
n=no. output bis
```

## Page 39
```text
Enample m= 110
lode Tree!-
0
m mI m2 m mm2 m mm2 mmm
M
=Au 110/6l
```

## Page 40
```text
CODE:
7th cydic code.sdX8th code tree.sdX
2 1 clc: clear:
5 =[1-10]:
7 6 disp(m);
8 9 00]=
10code=.[]: 11
13 12 fori=.1:length(m) u=m（i）:
14 15 xl=-modulo(u-+.state(1) +.state(2),2):
1E 17 x2=.modulo(u.+.state(2),2);
18 19 code=-[code-xl·x2];
20 21 end
22 23 disp("Convolutional.Encoded-Output:");
25 24 disp(code);
26 27 disp("Output-in.Pairs:"); for.i.=-1:2:length(code)
28 29 end -disp（string(code（i))·+-string(code（i+l))):
30
```

## Page 41
```text
OUTPUT:
Scilab2026.0.1Console "Input Message:"
"Convolutional Encoded Cutput: "Output in Pairs:" 1.1.0. 1. 0.1. 0.
"11" "01"
"01"
```

## Page 42
```text
EXPERIMENT-9
#AM :- Write a MATLAβ generating Convulatonal code Program oP wurobro zyt quwaidu! code Trellis.
eicientrepresentation conv-
olutional encoder Hhat shows the statetronsitions aver
Hime I+isderivcd drom thc code Jree but is more
compactandpractical dor implementedian.
In aconuulahon encoder, he etput depends oh:
> Previous bis stored in shyts registess (memory) Lurrentinput bit.
Trellis Representation:
Eoch node represents a statc >Each column represcnt aHime Hhe ehcoder.
>Eachbronch is (D or 2). Labeled with corresponding output bits.
Uneike the code +ree） the +relis merges identicalstatesreduciv
htxduo
Encoding Process:
1 Intieliaze Hhe Cncoder state usually all zeroes.
a) Input bits are Jed sequonHaly·
3)For each input:
Stutes
are generafed using Ggpo;uouhjod xoponzunb
The path through +rellis represents +he cncocled sequente.
Cocle Rate =
```

## Page 43
```text
#Erample m=01010101
m 3_ m2 O X X2 O Current State a Next State a
O
C
X= m田m_田m2
3田m
O du
Input bit1
302 s tdo po
01—1100100/010
```

## Page 44
```text
CODE:
7th cydic code.sa Xsth code tree.sd gth code relis.sdX
1 2 clc: clear:
3 牌 101010-101]
S 6 disp("lnput-Message:"):
diep(m):
10 9 00= code=[];
12 11 for i=I:length（m)
13 u=n（i);
15 14 xl= rodulo(u.+.state(1)+-state(2),2);
1E x2=odulo(u.+state(2),2):
17 18 code =.[code xl x2]:
19 20
21 end
22
23 24 disp(code):
25 26 disp("Output-in.Pairs:");
28 27 for i=l:2:length(code) disp(string(code(i)) + string(code(i+l))):
29end
30
```

## Page 45
```text
OUTPUT:
Sciaa2026.0.1Consoe iabessar anduru
"Convolutional Ehcoded Cutputt ... 1
"output in Pairs:" 0. 0.1.1.
00 "11"
#11# "01"
*01" "11"
"01* "11"
```

## Page 46
```text
EXPERIMENT -1O
encocing aneelecoding BCH code.
powexyue crror -correcting cocles capable
mulHole errors.
A Bch codeis clejined parameters Cn,k) where:
< n=length ceclceword
K=no. message bits
#Encoding process
7 Me ssaqe s represented as a polynemicd mC2)
)It smultip lied 2n-Kc
>The resulhs is durded by +he generator polynomial g(n)
((2n) = m(n). n-k+ R(x)
Where :> R(n) = remaindey.
#Decoding Process:
1)aecieve bolynomial r(~)
2)(ompute Syndrome values.
Use crrors locatoy polynomial t dind crror positions.
Correct thc errors·
# Error Correction Capabiliy
→ A BcH code can coyrect upts to tcarors :
t= dmin 2
dmin is the min hamin Dstovee
```

## Page 47
```text
BcH cocle
wih block tength )=u
t=3,
g（a)=L（M[m1）m2(2）,m3（(2）,my（n),mg（n）,m6（2)]
g(c)=LCM[m（n)m（(n).m()]
In GF (2°),
mCa)=25+n²+1
m2(n)= m(n)
+z+n++=(e)w
my(2n)=m2（n)
m5（n)=n+2y+2²+n+1
m(n)=mg()
g(2) =[m(n). mg(n).mg(n)]
g（()=2+2+0+2+n8+x++25+2²+2²+2+1
Ingo length(k)=n-mt
n2=31-6x3
31=2m-1=31-15,k=16
2m=32
m=5
比ence) it is ( 31)1e) triple- ces errorCorrecting Bch cocle.
```

## Page 48
```text
Encocling:- 2u15.m(a)
:（)Rg
r(0n)=n5m（2）.g()
(2++2+2++2²
C(2)=5m(n)+（x
Encoded Codcword:-
1011 0011011 01 6 1/1 1 01 000160/ 0/ 0 /
Decodiny
```

## Page 49
```text
7th cydic code.sd 2 1 clean: clc: 8th code tree.sd gth code trellis.sd 10th bch code.sci
4 3 n 31
E S n 1 一
小 0 7 n3g 1.10011010-11:
11 10 disp（nsg）:
12 13 010-01.01
15 14 terp [nsg.二ero8(1,r)]=
17 1E dividend =temp;
19 18 foz ifdividend(i)==1then 1:k
21 20 for-j=1:length(g) dividend（i-)-l)= xor(dividend(i+j-1).-g(j)):
23 22 end end
24 25 end
26 rem =dividend(k+l:n):
27 28 d19p（"Eericy.Bit3:"）:
30 29 disp（rem):
31 codeword-(msg rem]:
32 33 disp("Encoded-BoH.cod=vord:"):
35 34 uisp(codewozd):
36 recv=codeword:
37 38 disp("Received-Codevord:"):
39 disp(recv):
```

## Page 50
```text
40 41 dividend2=recv:
42 43 1
44 45 ifdividend2（i)==lthen forj=1:length(g)
4E 47 48 end end dividend2(i+j-l)=xor（dividend2（i+j-1),g(j));
49 50 end
51 52 syndrone=dividend2(k+l:
53 54 disp（syndrome): disp("Syndr
55 SE 57 58 else disp EYTOY othen
59 60 end disp("Error-Detected"
E1 62 E3 decoded=-recv(l:k):
E4 disp("Decoded-Message:" arldecndedi!
```

## Page 51
```text
OUTPUT:
Scist 202e 0.1 Conso
atiine 1. 0.1. 21 or executed riie D:\Irc\ioth bch code.sci 0. D. 0. Q.
Dndefined variabie: xor
```
