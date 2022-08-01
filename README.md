
local i=string.byte;local h=string.char;local c=string.sub;local N=table.concat;local E=table.insert;local s=math.ldexp;local P=getfenv or function()return _ENV end;local l=setmetatable;local r=select;local t=unpack or table.unpack;local d=tonumber;local function Q(f)local e,n,t="","",{}local a=256;local o={}for l=0,a-1 do o[l]=h(l)end;local l=1;local function i()local e=d(c(f,l,l),36)l=l+1;local n=d(c(f,l,l+e-1),36)l=l+e;return n end;e=h(i())t[1]=e;while l<#f do local l=i()if o[l]then n=o[l]else n=e..c(e,1,1)end;o[a]=e..c(n,1,1)t[#t+1],e,a=n,n,a+1 end;return table.concat(t)end;local d=Q('24F24E27524E24B27626L26M27326H26O27427524P27624E24827626E25G26Z26K26P26E27J27625Q27326Y26J26T27R24927625S26V27126T25R25M26C24E28027526226T26J27026M26Z26Z24E24227625X26V26O26X24Z26P26W24Z26226Z27V28927625U26P26Q26V26526P26O24E24527626028V26I26J26K26Z25V28H28I24627625T26O26Z24Z25M26V26R28I28K27526126P26Y26Q26F25V27326O27326X27O29627625Y26J26U2A92AA2AA27727627N27P24S24E24427629F29E28V25J26J28O2A527525U28V28G26O26R27326V2AZ2AI27626126124Z26326C24Z26126J26F26L2B127525P28G27326K25D28G26M26P24E29I2AS29P26Z29Q28H2AR24E25X26Z26M25L2AY28225W2AY2BN28L27C25V26V25U26J27R27K27526326E24Z26Z26E28I23X27625L26726525P24Z26725P25P25I24Z25L26225P26728T26226225G24E2CK27525X26725T2CU25U26Q25T25K24Z26526525I25Z24Z25Q26525Z25I2D427626225L25Y2CP25V25X2622DJ25Z25L25W26224Z2E12CW2DP27526525Q25T2CP25K25P2CW24Z25G25L2EE2642602632622E624E25N25L25Z2E22602672602CP26025L2CS24Z25R2D125P2EN25X25Z25P2E22DG2EE2EA26225X2CV2DX2F32D524E25U25T2CO24Z2F72FL25V25Z26525L24Z25S2EP2EM2FH25S2622EP24Z25X25W2FL2DZ25N2CP25Z25W2E52FH2FC2EY2CV26526326024Z25N2DZ2CP2CO2CR2EN2G825L2GH26425O2642ES25O26326324Z25T25Q25X2612EN2FP25P2FD2CW2642642B82B32B42FU25L2DO2GB2672FY2B826326125O24Z25J26326725Y24Z2FP2DR2EN2ET25S2B42DR2602B425X25N25J25J24Z2602HP2FG27625Z2I42CZ2CW2EE25Y2GX2GY2FU26225K2EN26725I25I2CP25X25T25T2FS2CW25P2652GZ2E025P24C27I27523224H2AD27527B26V26K2BC2J324A27626X27329Q28X27525Q26Q27326F27O2BC2972AS26P27127326Q2JL2JN2A42JE2D628326T24E23Y28126P26I25A27325A26G2JV26V26Y25A26T26Z26F25B24E2J227525D2H324D28L2KI2BD24E25P26I2BH26I27O2B926V2JJ2KU26Z26I29329D2K427625P26Z26O26Y25S2K726V26W28327326I26V2942J724E29O26I26Q28I2472CL26U26V2KY29126L26I24E2K02LO2CH2M028A2KU26J27127126Z26L2BC2BO24E26229C2LJ2LL2952KM24E24V24U24E2LT27525K2AY26Q2KF2BW26F2M127626H2AY2M027I2DO27625027623R27623W27527427F24E2NA2KL2NG2752NF2KQ2KQ2NI2752JE2M22NF2782782NM27S2CC2NE2752802M62NF29I2ME2NF2LT2MQ2NW2B12AJ2NT2972JR2O628K29S2O624324E2OG2NT24024E2OK2NT24124E2OO2NT2K52K52NT23Z24E2OV2NT2NA2NF2O62CK2FH2NF23U24E2P52NT23V24E2P92NT23S24E2PD2NT23T24E2PH2NT23Q24E2PL2NT2N82N82NT23O24E2PS2NT23P24E2PW2NT23M24E2Q02NT23N24E2Q42NT23K24E2Q82NT23L24E2QC2NT25A24E2QG2NT2KK2KK2NT25824E2QN2J32752QN27423W2JE27425927I2PH2J22ML2NJ24E2562QQ2M22J32KQ2J22782R62H327F2972ME2752482NA27424R24E27429I24A2NS24E2RK2QT2M22572N92PW29I2542762QI2O124E2552QH2752S12522S42C429I2532O62AJ2N62J329I2AJ2742RB2RL2NE2Q829I2512RZ2OG2S124Y27J2NA2802602SK2RN2RP2SW2QT2SM24E2RY27525A2SS2S124Z2S82S124W2SC24E24X2QQ2OB2KQ2MO2A52MO24V24E2TJ2972AH24T2TN27529724Q2RQ27I29I2972QT2S524E2SO2T52752J229I2SS2P024E2RU2NN27I2RC2QH2LT2NC24E2QX2482OK2KQ2N62742J22RO2N52SK23W2Q82KQ2U32QH2OG2NK24E2SS2RH24E2KQ25S2SK2UP2RP2V52SI2RP25M2US2UU2T32RZ2J22UZ2S32QI2UZ2S72VK2V324E2SB2NQ24E24O2QQ2KQ2782T12VO27H2762SO2KQ2UH2UQ27525Z2SK2PT2762ND2MY2NI2QA2W72KL2QX2WA2752T42NG27F2PU2WE');local o=bit and bit.bxor or function(l,n)local e,o=1,0 while l>0 and n>0 do local c,a=l%2,n%2 if c~=a then o=o+e end l,n,e=(l-c)/2,(n-a)/2,e*2 end if l<n then l=n end while l>0 do local n=l%2 if n>0 then o=o+e end l,e=(l-n)/2,e*2 end return o end local function n(e,l,n)if n then local l=(e/2^(l-1))%2^((n-1)-(l-1)+1);return l-l%1;else local l=2^(l-1);return(e%(l+l)>=l)and 1 or 0;end;end;local l=1;local function e()local e,c,n,a=i(d,l,l+3);e=o(e,158)c=o(c,158)n=o(n,158)a=o(a,158)l=l+4;return(a*16777216)+(n*65536)+(c*256)+e;end;local function f()local e=o(i(d,l,l),158);l=l+1;return e;end;local function a()local n,e=i(d,l,l+2);n=o(n,158)e=o(e,158)l=l+2;return(e*256)+n;end;local function Z()local l=e();local e=e();local c=1;local o=(n(e,1,20)*(2^32))+l;local l=n(e,21,31);local e=((-1)^n(e,32));if(l==0)then if(o==0)then return e*0;else l=1;c=0;end;elseif(l==2047)then return(o==0)and(e*(1/0))or(e*(0/0));end;return s(e,l-1023)*(c+(o/(2^52)));end;local s=e;local function Q(e)local n;if(not e)then e=s();if(e==0)then return'';end;end;n=c(d,l,l+e-1);l=l+e;local e={}for l=1,#n do e[l]=h(o(i(c(n,l,l)),158))end return N(e);end;local l=e;local function s(...)return{...},r('#',...)end local function N()local d={};local o={};local l={};local i={d,o,nil,l};local l=e()local c={}for n=1,l do local e=f();local l;if(e==1)then l=(f()~=0);elseif(e==2)then l=Z();elseif(e==0)then l=Q();end;c[n]=l;end;for l=1,e()do o[l-1]=N();end;i[3]=f();for i=1,e()do local l=f();if(n(l,1,1)==0)then local o=n(l,2,3);local t=n(l,4,6);local l={a(),a(),nil,nil};if(o==0)then l[3]=a();l[4]=a();elseif(o==1)then l[3]=e();elseif(o==2)then l[3]=e()-(2^16)elseif(o==3)then l[3]=e()-(2^16)l[4]=a();end;if(n(t,1,1)==1)then l[2]=c[l[2]]end if(n(t,2,2)==1)then l[3]=c[l[3]]end if(n(t,3,3)==1)then l[4]=c[l[4]]end d[i]=l;end end;return i;end;local function f(l,e,a)local n=l[1];local e=l[2];local l=l[3];return function(...)local o=n;local h=e;local c=l;local l=s local e=1;local l=-1;local N={};local i={...};local d=r('#',...)-1;local l={};local n={};for l=0,d do if(l>=c)then N[l-c]=i[l+1];else n[l]=i[l+1];end;end;local l=d-c+1 local l;local c;while true do l=o[e];c=l[1];if c<=21 then if c<=10 then if c<=4 then if c<=1 then if c>0 then n[l[2]][l[3]]=l[4];else n[l[2]]=a[l[3]];end;elseif c<=2 then local a;local c;n[l[2]]=n[l[3]][l[4]];e=e+1;l=o[e];n[l[2]]=n[l[3]][l[4]];e=e+1;l=o[e];c=l[2];a=n[l[3]];n[c+1]=a;n[c]=a[l[4]];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];c=l[2]n[c](t(n,c+1,l[3]))elseif c==3 then n[l[2]]=#n[l[3]];else n[l[2]]=l[3];end;elseif c<=7 then if c<=5 then e=l[3];elseif c==6 then local e=l[2];local o=n[e];for l=e+1,l[3]do E(o,n[l])end;else for l=l[2],l[3]do n[l]=nil;end;end;elseif c<=8 then n[l[2]]=f(h[l[3]],nil,a);elseif c==9 then n[l[2]]=n[l[3]]+l[4];else local e=l[2]n[e](t(n,e+1,l[3]))end;elseif c<=15 then if c<=12 then if c==11 then n[l[2]]=#n[l[3]];else n[l[2]]=n[l[3]];end;elseif c<=13 then n[l[2]]=n[l[3]][l[4]];elseif c>14 then n[l[2]]=n[l[3]]+l[4];else local c=l[2];local a=l[4];local o=c+2 local c={n[c](n[c+1],n[o])};for l=1,a do n[o+l]=c[l];end;local c=c[1]if c then n[o]=c e=l[3];else e=e+1;end;end;elseif c<=18 then if c<=16 then local l=l[2]n[l](n[l+1])elseif c==17 then do return end;else if(n[l[2]]==n[l[4]])then e=e+1;else e=l[3];end;end;elseif c<=19 then n[l[2]]=l[3];elseif c==20 then n[l[2]][l[3]]=l[4];else local o=l[2];local a=l[4];local c=o+2 local o={n[o](n[o+1],n[c])};for l=1,a do n[c+l]=o[l];end;local o=o[1]if o then n[c]=o e=l[3];else e=e+1;end;end;elseif c<=32 then if c<=26 then if c<=23 then if c>22 then local c;local f;local t;for l=l[2],l[3]do n[l]=nil;end;e=e+1;l=o[e];n[l[2]]=a[l[3]];e=e+1;l=o[e];n[l[2]]=n[l[3]];e=e+1;l=o[e];t=l[2]f={n[t](n[t+1])};c=0;for l=t,l[4]do c=c+1;n[l]=f[c];end e=e+1;l=o[e];e=l[3];else local e=l[2]local c={n[e](n[e+1])};local o=0;for l=e,l[4]do o=o+1;n[l]=c[o];end end;elseif c<=24 then n[l[2]]=n[l[3]][l[4]];elseif c==25 then n[l[2]]={};else do return end;end;elseif c<=29 then if c<=27 then local f;local c;n[l[2]]=a[l[3]];e=e+1;l=o[e];n[l[2]]=n[l[3]][l[4]];e=e+1;l=o[e];n[l[2]]=n[l[3]][l[4]];e=e+1;l=o[e];c=l[2];f=n[l[3]];n[c+1]=f;n[c]=f[l[4]];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];c=l[2]n[c](t(n,c+1,l[3]))e=e+1;l=o[e];e=l[3];elseif c>28 then local e=l[2];local o=n[l[3]];n[e+1]=o;n[e]=o[l[4]];else local o=l[2]local c={n[o](n[o+1])};local e=0;for l=o,l[4]do e=e+1;n[l]=c[e];end end;elseif c<=30 then n[l[2]]=a[l[3]];elseif c==31 then n[l[2]]={};else local o=l[2];local e=n[l[3]];n[o+1]=e;n[o]=e[l[4]];end;elseif c<=38 then if c<=35 then if c<=33 then local e=l[2]n[e](t(n,e+1,l[3]))elseif c>34 then n[l[2]]=f(h[l[3]],nil,a);else for l=l[2],l[3]do n[l]=nil;end;end;elseif c<=36 then local e=l[2];local o=n[e];for l=e+1,l[3]do E(o,n[l])end;elseif c>37 then local l=l[2]n[l](n[l+1])else n[l[2]]=n[l[3]];end;elseif c<=41 then if c<=39 then e=l[3];elseif c>40 then n[l[2]]();else if(n[l[2]]==n[l[4]])then e=e+1;else e=l[3];end;end;elseif c<=42 then local a;local c;n[l[2]]={};e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];c=l[2];a=n[c];for l=c+1,l[3]do E(a,n[l])end;elseif c>43 then local f;local c;n[l[2]]=n[l[3]][l[4]];e=e+1;l=o[e];c=l[2];f=n[l[3]];n[c+1]=f;n[c]=f[l[4]];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];n[l[2]]={};e=e+1;l=o[e];n[l[2]][l[3]]=l[4];e=e+1;l=o[e];n[l[2]][l[3]]=l[4];e=e+1;l=o[e];n[l[2]][l[3]]=l[4];e=e+1;l=o[e];c=l[2]n[c](t(n,c+1,l[3]))e=e+1;l=o[e];n[l[2]]=a[l[3]];e=e+1;l=o[e];n[l[2]]=n[l[3]][l[4]];e=e+1;l=o[e];n[l[2]]=l[3];e=e+1;l=o[e];e=l[3];else n[l[2]]();end;e=e+1;end;end;end;return f(N(),{},P())();
