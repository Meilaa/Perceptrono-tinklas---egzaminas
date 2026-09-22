**Rekurentinis dirbtinis neuroninis tinklas – Backpropagation**

Pagal pateiktą neuroninio tinklo struktūrą sužymėti koeficientus, išvesti tinklo atsako ir svorių atnaujinimo formules bei jas realizuoti MATLAB aplinkoje.

**Tinklo struktūra**

Realizuotas trijų sluoksnių neuroninis tinklas su grįžtamuoju ryšiu:

2 įėjimai → 2 neuronai → 3 neuronai → 1 išėjimas

Įėjimai: x(n) ir ankstesnis tinklo išėjimas y(n−1).

Visuose sluoksniuose naudojama sigmoidinė aktyvacijos funkcija. Tinklas turi 13 svorių ir 6 bias koeficientus.

**Tinklo mokymas**

Mokymui naudojamas Backpropagation algoritmas:

Apskaičiuojamas tinklo išėjimas (Feedforward).

Nustatoma klaida tarp norimo ir gauto atsako.

Apskaičiuojami neuronų klaidos gradientai.

Atnaujinami visų sluoksnių svoriai ir bias koeficientai.

Mokymosi greitis: η = 0.1 Mokymo epochų skaičius: 80 000

**MATLAB realizacija**

Programa parašyta be matricinių operacijų, kiekvieno neurono skaičiavimus ir svorių atnaujinimą pateikiant atskirai.

Kadangi užduotyje konkretūs mokymo duomenys nepateikti, tinklo veikimui pademonstruoti naudojami pavyzdiniai įėjimo duomenys ir sinusine funkcija apibrėžtas norimas atsakas.

Grįžtamasis ryšys realizuojamas dabartinį tinklo išėjimą naudojant kaip kito laiko žingsnio įėjimą.
